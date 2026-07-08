# Tool 2: Dreamweaver — Unreasonable Hospitality Idea Generator
**Tagline:** Give a rep a customer name and a moment — get back an idea that makes the customer feel like the only customer in the world.

---

## What It Is

An AI-powered idea generator that takes a customer context and produces specific, creative, actionable "unreasonable hospitality" moments — gestures that go far beyond what the customer expects and cement Simpson Strong-Tie's relationship at a human level.

"Unreasonable hospitality" is the operating philosophy: don't just serve customers well, make them feel genuinely cared for in ways that surprise them.

**Input:** Customer name, relationship context, upcoming touchpoint or milestone
**Output:** 3–5 concrete, specific, executable ideas — ranked from quick/easy to wow/memorable

---

## Why This Matters

**For NPS:** Customers who feel genuinely remembered and valued don't just renew — they refer. NPS improvement comes from the emotional layer, not just the transactional one.

**For rep development:** Reps who learn to think about customers this way become relationship sellers, not transaction sellers. This tool teaches the mindset by modeling it.

**For competitive differentiation:** Building materials is a commodity-adjacent market. The product matters, but the relationship is what keeps a customer from taking a competitor's call. This is the relationship builder.

---

## How It Works

### The Prompt Interface

```
Rep inputs:
  Customer name: [Acme Construction]
  Key contact: [Jim Torres, Project Manager]
  What we know about Jim: [Has a 10-year-old who plays soccer. Just wrapped
    a major project in Riverside. Big Dodgers fan. Always mentions being
    overwhelmed with paperwork.]

  Upcoming moment: [Annual review call next Thursday]

Dreamweaver output:
  IDEA 1 (Quick, this week): 
    Send Jim a handwritten note thanking him specifically for the Riverside 
    project — mention one detail about the job that shows you were paying 
    attention. "The timeline you managed on that foundation work was 
    impressive." Takes 10 minutes. Costs a stamp. Lands like $1,000.

  IDEA 2 (For the call):
    Open the annual review by asking about his son's soccer season before 
    you go anywhere near numbers. One minute of genuine interest before 
    business. Then: "You mentioned paperwork is a constant headache — I 
    want to show you one feature of the customer portal that eliminates 
    3 steps from your order process. Here's what it looks like."

  IDEA 3 (This quarter):
    Dodgers fan + baseball season = obvious. Send him two tickets to a game 
    with a note: "For you and your son — no agenda, just a thank you for 
    10+ years of partnership." Check SST gifting policy first.

  IDEA 4 (Long game):
    Jim mentioned paperwork overwhelm. Build him a custom order template 
    in the customer portal pre-loaded with his most frequent SKUs. Deliver 
    it as a gift on the next call: "I had our team build this specifically 
    for your workflow." He didn't ask for it. That's the point.
```

---

## Build Approach

**Phase 1 — Core prompt engine (1 week)**
- A well-engineered system prompt that understands "unreasonable hospitality" deeply
- Input form: customer name, key contacts, relationship notes, upcoming moment
- Output: structured ideas with effort level, cost, and timing

**Phase 2 — Customer context integration (1 week)**
- Pull context from contacts.json where available
- Rep can add quick notes before generating (recent conversation, personal detail just learned)
- Ideas are tagged: quick win / this week / this quarter / long game

**Phase 3 — Idea library (ongoing)**
- Every idea a rep actually executes gets logged with the outcome
- Over time, builds a library of what has worked with which customer types
- Steve can share standout examples in team meetings

**Phase 4 — Team ritual integration (ongoing)**
- Weekly team meeting agenda item: "One unreasonable hospitality moment from this week"
- Dreamweaver becomes part of call prep, not just a standalone tool

---

## Files to Build

```
/dreamweaver/
  SYSTEM_PROMPT.md    ← The core AI prompt that defines hospitality philosophy
  input_template.md   ← What reps fill in to generate ideas
  idea_library.json   ← Logged executed ideas and outcomes (gitignored)
  examples/           ← Sample inputs and outputs for onboarding
```

---

## Success Metrics

| Metric | Baseline | Target | Timeline |
|--------|---------|--------|----------|
| NPS score | 98% target | Maintain + sustain | Ongoing |
| Customer-mentioned personal moments (call notes) | [Baseline] | Increasing | 90 days |
| Rep confidence in relationship conversations | [Survey] | Improved | 60 days |
| Ideas executed per week (team total) | 0 | 5+ | 30 days |

---

## The Pitch to Zack

> "I'm building a tool for the team called Dreamweaver — it's an AI-powered unreasonable hospitality idea generator. Rep inputs a customer name and a moment, and gets back specific, creative ways to make that customer feel like the most important customer we have. It's how we defend NPS and build the kind of relationships that make switching feel unthinkable."

---

## Why This Name

Dreamweaver: the tool helps reps weave the customer's world into the customer experience. It's not generic hospitality advice — it's custom, personal, and specific to the relationship in front of them.
