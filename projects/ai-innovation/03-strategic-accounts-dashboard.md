# Tool 3: Strategic Accounts Dashboard
**Tagline:** Every strategic account, visible at a glance — with AI surfacing what needs attention before it becomes a problem.

---

## What It Is

An AI-powered dashboard that gives Steve (and eventually leadership) a live picture of every strategic account in the Southwest territory: health, engagement, last touch, open opportunities, risk signals, and AI-generated next actions.

This is not a CRM replacement. It's an intelligence layer on top of what already exists — synthesizing data from the CRM, rep notes, customer portal usage, and contact history into a clear, actionable view.

---

## Why This Matters

**For Steve:** Managing key account relationships across a $340M territory with 19 reps is impossible without a system. Right now, account health lives in people's heads. This makes it explicit, trackable, and proactive.

**For leadership visibility:** This dashboard is the kind of tool that gets shown in QBRs and exec reviews. It's not just useful — it's presentable. Zack and Phil see a leader who built something, not just managed something.

**For the business:** Customer retention is the cheapest growth. Every at-risk account caught early is revenue protected. Every relationship deepened is a competitor kept out.

---

## How It Works

### The Dashboard View (Steve's Interface)

```
STRATEGIC ACCOUNTS DASHBOARD — Southwest Region
Updated: [Date]

ACCOUNT HEALTH SUMMARY
  Total strategic accounts: [N]
  Green (healthy, engaged): [N]
  Yellow (needs attention): [N]
  Red (at-risk, Steve engaged): [N]

TOP 5 ACCOUNTS NEEDING ATTENTION
  1. [Account] — [Contact] — Last touch: 23 days — Risk: [Portal unused 60 days]
     AI action: "Call Jim Torres. Mention the Riverside project. Offer the custom
     order template you built. This is a renewal account — don't let it go cold."
  
  2. [Account] — [Contact] — Last touch: 18 days — Risk: [New stakeholder appeared]
     AI action: "Sarah mentioned a new VP of Procurement started last month.
     Get introduced before that person builds a relationship with a competitor."

ACCOUNT PORTFOLIO
  | Account | Contact | Rev | Last Touch | Portal | Health | Next Action |
  |---------|---------|-----|------------|--------|--------|-------------|
  | [Name]  | [Name]  | $Xm | X days     | Active | 🟢     | [Action]    |
  | [Name]  | [Name]  | $Xm | X days     | None   | 🟡     | [Action]    |

INTELLIGENCE FLAGS (AI-generated)
  - [Account]: Portal usage dropped 40% this month — investigate before renewal
  - [Account]: Contact hasn't responded to two emails — escalate or re-route
  - [Account]: Just awarded a major project in [city] — opportunity to expand
```

### AI Intelligence Layer

The AI synthesizes across data points to generate signals a human might miss:
- **Staleness detection:** "You haven't touched this $200K account in 31 days"
- **Portal drop signals:** "Portal usage declining = customer disengagement risk"
- **Opportunity flags:** "Regional construction permit spike in their market — call now"
- **New stakeholder alerts:** "Decision-maker changed — relationship is at zero"
- **Win pattern recognition:** "Accounts that use portal weekly have 22% higher retention"

---

## Build Approach

**Phase 1 — Static dashboard (2 weeks)**
- Manual data input: Steve or reps update account health, last touch, portal usage weekly
- Simple markdown dashboard with color coding and AI-generated action prompts
- No integration required — just structured data in a clean format

**Phase 2 — AI intelligence layer (2 weeks)**
- Feed account data through Claude to generate specific next-action recommendations
- Add pattern detection: identify what healthy accounts have in common vs. at-risk accounts
- Weekly auto-summary Steve can share with Zack

**Phase 3 — Data integration (ongoing)**
- Connect to CRM export (CSV or API if available)
- Connect to customer portal usage data
- Automate the data refresh so the dashboard is always current

**Phase 4 — Leadership view (Q4 2026)**
- A clean one-page summary version for Zack / exec reviews
- Shows team's strategic account health at a portfolio level
- Steve presents this in QBR — this is the visibility play

---

## Files to Build

```
/strategic-accounts/
  dashboard.md          ← Live dashboard (updated weekly)
  accounts.json         ← Account data structure (gitignored — customer data)
  intelligence.md       ← AI-generated flags and recommendations
  templates/
    account_profile.md  ← Structure for each strategic account
    weekly_summary.md   ← Format for Zack update
```

---

## Data Structure per Account

```json
{
  "id": "acct-001",
  "name": "Company Name",
  "key_contact": "Name, Title",
  "annual_revenue": "$XM",
  "tier": 1,
  "last_contact_date": "2026-07-01",
  "portal_status": "active | inactive | declining",
  "portal_last_used": "2026-06-28",
  "health": "green | yellow | red",
  "renewal_date": "2026-12-01",
  "open_opportunities": [],
  "risk_flags": [],
  "ai_next_action": "",
  "rep_owner": "Rep Name",
  "notes": ""
}
```

---

## Success Metrics

| Metric | Baseline | Target | Timeline |
|--------|---------|--------|----------|
| At-risk accounts caught before churn | Unknown | Track and improve | Ongoing |
| Average days since last touch (Tier 1 accounts) | [Baseline] | Under 14 days | 60 days |
| Customer retention rate | [Baseline] | Maintain + improve | Ongoing |
| Portal active usage across strategic accounts | [Baseline] | +X% | 90 days |

---

## The Pitch to Zack / Phil

> "I built a Strategic Accounts Dashboard for the Southwest territory — it gives me (and you) a live picture of every key account: health, engagement, portal usage, risk signals, and AI-generated next actions. I want to present this in our next QBR. It's the kind of visibility I think we should have at a regional level across all our managers."

That last sentence is Senior Manager of Sales Operations language. That's the target.
