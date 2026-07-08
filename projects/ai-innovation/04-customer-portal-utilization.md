# Tool 4: Customer Portal Utilization Plan & Training
**Tagline:** Every customer on the portal, using it consistently — because the training met them where they are.

---

## What It Is

An AI-powered system that creates personalized Customer Portal adoption plans and training content for each customer, based on their industry, usage patterns, order behavior, and specific friction points.

Customer Portal utilization is a current Q priority for Steve's team. The gap isn't product — it's adoption. Customers don't use the portal because nobody has made it feel worth using *for them specifically*. This tool fixes that.

---

## Why This Matters

**For the metric:** Customer Portal utilization is a named KPI. Moving this number is a direct business result Steve owns.

**For order accuracy:** Customers who order through the portal make fewer errors than customers who call in. Higher portal adoption = higher order accuracy = better NPS. These metrics compound.

**For rep efficiency:** A rep who has 40% of their customers self-serving through the portal has more time for strategic relationship work, not order entry and follow-up.

**For the customer:** A customer who uses the portal has faster orders, better tracking, and fewer mistakes. The value is real — the training just hasn't landed that way before.

---

## The Problem with Generic Training

Most portal training is:
- Generic (same deck for every customer)
- Company-centric (here's what the portal does, not here's what it does *for you*)
- One-and-done (no follow-up, no adoption tracking)

This tool makes training:
- Specific to the customer's actual order patterns
- Framed around what the customer saves/gains, not what the rep wants them to do
- Ongoing — with check-ins tied to actual usage data

---

## How It Works

### Customer Adoption Plan Generator

**Input:**
```
Customer: [Acme Construction]
Contact: [Jim Torres, Project Manager]
Industry: [Commercial construction — GC]
Current portal status: [Has login, used twice in 6 months]
Most common order types: [Structural connectors, anchor bolts — repeat SKUs]
Known friction: [Jim says logging in is annoying and he's not sure it saves time]
Upcoming touchpoint: [Annual review call Thursday]
```

**Output — Personalized Adoption Plan:**
```
ACME CONSTRUCTION — PORTAL ADOPTION PLAN

Jim's situation: Jim has used the portal twice. He's skeptical it saves time.
His primary order type is repeat SKUs — this is the perfect portal use case.

STEP 1 — This call (Thursday):
  Don't demo the portal. Ask Jim one question: "How long does your typical
  connector order take from call to confirmation?" 
  [He'll say 15-20 minutes. The portal takes 3.]
  Then offer to show him one thing — not a tour, one thing — that cuts that
  time in half. That's your in.

STEP 2 — Before the call (prep):
  Build Jim a saved order template in the portal pre-loaded with his 15 most
  frequent SKUs and standard quantities. Name it "Acme Standard Order."
  Show it to him cold on the call. He didn't ask for it. That's the point.

STEP 3 — 30 days post-call:
  Check portal usage data. If Jim used it 3+ times: call to celebrate.
  "You're already saving X hours a month." 
  If Jim hasn't used it: "Quick question — what got in the way?"
  Solve the actual friction, don't re-pitch the product.

STEP 4 — 60 days:
  Jim is now a portal user. Ask him: "Is there a project manager you know
  who still calls in orders?" Referral to portal adoption from peer to peer
  is 3x more effective than rep-to-customer.

TRAINING CONTENT TO CREATE FOR JIM:
  - 90-second video: "How Jim Torres orders in 3 minutes vs. 20"
  - One-page PDF: "Your Acme Standard Order — step by step"
  - Quick reference card: the 5 things Jim will actually use
```

---

## Build Approach

**Phase 1 — Adoption plan generator (1 week)**
- AI prompt that takes customer context and generates a specific, staged adoption plan
- Reps run this before any customer call where portal is on the agenda
- No integration needed — context-driven, manually input

**Phase 2 — Training content templates (1 week)**
- AI-generated customer-specific one-pagers and quick reference guides
- Framed around the customer's workflow, not the portal's features
- Reps can customize and send directly

**Phase 3 — Usage tracking integration (2 weeks)**
- Pull portal usage data per customer (if available from the platform)
- Flag customers who have access but zero/low usage
- Auto-generate outreach prompts: "These 8 customers have logins but haven't logged in in 30 days — here's the personalized approach for each"

**Phase 4 — Team adoption ritual (ongoing)**
- Weekly team meeting: "Portal adoption update — who moved this week?"
- Rep leaderboard: portal-active customers per rep
- Share success stories: "Sarah got Hendricks Construction to 100% portal for repeat orders — here's how"

---

## Files to Build

```
/customer-portal/
  adoption_plan_generator.md    ← AI prompt template for generating plans
  customer_plans/               ← One plan per strategic customer (gitignored)
  training_templates/
    onepager_template.md        ← AI-generated customer-specific one-pager
    quick_reference_template.md ← Quick reference card template
  tracking/
    usage_log.json              ← Portal adoption status per customer
    adoption_dashboard.md       ← Team-level adoption view
```

---

## Success Metrics

| Metric | Baseline | Target | Timeline |
|--------|---------|--------|----------|
| Customer Portal utilization rate | [Current %] | +X% | 90 days |
| Strategic accounts on portal (active) | [Baseline] | 80%+ | Q4 2026 |
| Order accuracy rate | 99.35% target | Maintain + improve | Ongoing |
| Rep time on order entry (saved) | [Baseline] | Measurable reduction | 60 days |

---

## The Pitch to Zack

> "Portal utilization is a Q priority and we've been treating it like a generic training problem. I built a system that generates a personalized adoption plan for each strategic customer — based on their actual order patterns and where they get stuck. We're not showing them the portal. We're showing them what the portal does for *them*."

That's a different level of thinking than "we need to train customers on the portal."
