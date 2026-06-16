# Framework: AI Tool & Vendor Evaluation for Sales

**Purpose:** A structured approach for evaluating AI tools and vendors in a sales context — for Steve's own team's productivity or as a perspective when customers ask.

---

## Why This Framework Exists

AI tools for sales are proliferating rapidly. The gap between vendor marketing and actual value is enormous. Steve needs to be able to evaluate these tools as a buyer (for his team), as a credible conversationalist (with customers who are evaluating tech), and as a thought leader (in the Director promotion conversation, being the person who led the team's AI adoption is meaningful).

---

## Evaluation Criteria

### 1. Capability (Does it actually do what it claims?)

**Questions to answer:**
- What specific problem does this solve? Is that problem real for Steve's team?
- Can you see a live demo with your actual data (not vendor-prepared data)?
- What's the failure mode? When does it not work?
- How does it handle edge cases in construction/B2B sales?
- What does the AI actually do vs. what requires human judgment?

**Weight:** 30% of decision

**Scoring (1-5):**
- 5: Demonstrably solves a real problem, live demo is convincing with real scenarios
- 4: Solid capability with one or two meaningful gaps
- 3: Works for some use cases but not the core problem
- 2: Claims don't hold up under real-world testing
- 1: Doesn't do what it says

---

### 2. Integration (Will it actually fit into the workflow?)

**Questions to answer:**
- Does it integrate with the existing CRM (Salesforce, HubSpot, etc.)?
- Is the integration native (deep) or surface-level (just data sync)?
- How much workflow change does adoption require?
- How long until a rep actually uses it naturally vs. feeling like extra work?
- What breaks if the integration fails or the vendor changes their API?

**Weight:** 25% of decision

**Scoring (1-5):**
- 5: Native integration, minimal workflow disruption, actually reduces steps
- 4: Good integration, requires some adjustment
- 3: Works but requires meaningful workflow change
- 2: Bolted on, creates more work than it saves early on
- 1: Doesn't integrate; requires manual data movement

---

### 3. Security & Compliance (Can we trust it with customer data?)

**Questions to answer:**
- Where does customer data go? Who can see it?
- Is it SOC 2 Type II certified?
- Does it train its models on customer data by default? Can you opt out?
- GDPR/CCPA compliance if relevant?
- What's the data retention policy?
- Has it passed a security review? By whom?
- What happens to data if you cancel?

**Weight:** 20% of decision (non-negotiable floors: SOC 2, no training on customer data without opt-in)

**Scoring (1-5):**
- 5: SOC 2 certified, no training on customer data, clear data policies, easy to verify
- 4: Strong security posture with one gap that can be managed
- 3: Adequate but requires additional due diligence
- 2: Gaps that would require escalation to legal/IT
- 1: Fundamental security concerns — don't proceed

**Hard stops (automatic reject):**
- Uses customer data for model training without explicit opt-in
- No SOC 2 or equivalent certification
- Unable to answer where data is stored
- No data deletion process on cancellation

---

### 4. Cost (Is the value worth the price?)

**Questions to answer:**
- What is the total cost of ownership? (License + implementation + training + ongoing maintenance)
- How is it priced? (Per seat, per usage, flat fee?)
- What's the cost per rep per month?
- What productivity gain is needed to break even?
- Are there hidden costs (additional modules, support tiers, API usage fees)?
- What's the pricing in year 2 and beyond? Is it contractually locked?

**Weight:** 15% of decision

**ROI Calculation:**

```
Monthly cost per rep: $[X]
Hours saved per rep per month: [X] hours
Value of one rep hour: [Annual OTE / 2000 working hours]
Monthly value per rep: [Hours saved x hourly value]
Monthly ROI per rep: [Monthly value - Monthly cost]
Break-even timeline: [When cumulative savings exceeds implementation cost]
```

**Scoring (1-5):**
- 5: Clear positive ROI with conservative assumptions in under 3 months
- 4: Positive ROI, 3-6 month payback
- 3: Positive ROI but 6-12 month payback requires assumptions
- 2: ROI unclear or requires optimistic assumptions
- 1: Cost exceeds plausible benefit

---

### 5. Vendor Stability (Will they be here in 2 years?)

**Questions to answer:**
- How long has the company been operating?
- How many enterprise customers? (Reference-able ones?)
- What's their funding situation? (If startup — how much runway?)
- Are they venture-backed? What stage?
- Who are their major customers? Do they include companies like ours?
- What's the leadership team's track record?
- What's the contract term and what happens if they shut down?

**Weight:** 10% of decision

**Scoring (1-5):**
- 5: Established, profitable, or well-funded with multiple references in our industry
- 4: Funded, growing, and has comparable customers
- 3: Early-stage but credible; manageable risk with a short initial contract
- 2: Concerning stability signals; short contract only with clear exit provisions
- 1: Real risk of shutdown; avoid unless absolutely unique capability

---

## Scoring Matrix

| Vendor | Capability (30%) | Integration (25%) | Security (20%) | Cost (15%) | Stability (10%) | Weighted Score |
|--------|-----------------|-------------------|----------------|------------|-----------------|----------------|
| [Vendor A] | /5 | /5 | /5 | /5 | /5 | [Calc] |
| [Vendor B] | /5 | /5 | /5 | /5 | /5 | [Calc] |
| [Vendor C] | /5 | /5 | /5 | /5 | /5 | [Calc] |

**Weighted score formula:**
`(Cap × 0.30) + (Int × 0.25) + (Sec × 0.20) + (Cost × 0.15) + (Stab × 0.10)`

**Decision thresholds:**
- Score 4.0+: Proceed with implementation
- Score 3.0–3.9: Pilot with limited reps, reassess at 60 days
- Score 2.0–2.9: Decline or require significant concessions
- Score below 2.0: Decline

---

## Questions to Ask Vendors

### Capability Questions
1. "Show me the tool handling [specific scenario from our sales process] — with realistic data, not a demo environment."
2. "What percentage of [promised functionality] works out of the box vs. requiring configuration?"
3. "What are the top 3 ways customers are disappointed by your tool after implementation?"
4. "Who is your best customer in B2B/construction sales? Can I speak with them directly?"

### Integration Questions
5. "Walk me through the integration with [our CRM]. What's native vs. webhook vs. manual?"
6. "What's the typical time from contract to reps actually using it? (Not 'go live' — actually using it)"
7. "What breaks if we change our CRM configuration?"

### Security Questions
8. "Are you SOC 2 Type II certified? Can you share the report?"
9. "Does our data train your models? Exactly what does that mean for us?"
10. "Walk me through what happens to our data if we cancel."
11. "Have you passed a security review for a Fortune 500 company? Who?"

### Cost Questions
12. "What's the all-in cost for [our team size] over 3 years, including implementation?"
13. "What does the pricing look like in year 2? Is that contractually locked?"
14. "What does the average customer spend on services beyond the license fee?"

### Stability Questions
15. "What's your current ARR and how has it grown in the last 12 months?"
16. "Who are your enterprise customers that I could call as a reference?"
17. "What happens to our data and service if your company is acquired or shuts down?"

---

## Red Flags

Stop the evaluation if you see any of these:

**Capability red flags:**
- Can't demo with realistic data before you sign
- Avoids specific questions about limitations
- Customer references are coached or unusually similar to vendor talking points
- Product roadmap is mostly future features, not current value

**Integration red flags:**
- "Simple integration" turns into "3-month implementation project" when you dig
- Requires a dedicated admin to maintain
- Their "CRM integration" is actually just CSV export/import

**Security red flags:**
- Can't answer where data is stored
- Ambiguous language about training data ("we use data to improve our models")
- No SOC 2 or equivalent
- Data deletion process is unclear or takes months

**Vendor red flags:**
- Pressure tactics to sign before a "deadline" in the first meeting
- Unable to provide customer references in your industry
- Pricing changes dramatically between first discussion and final quote
- Key people left recently (check LinkedIn before signing)
- Contract terms bury auto-renewal with a short cancellation window

---

## Implementation Considerations

Before signing, have answers to these:

**Adoption:**
- Who owns the rollout? (Steve, ops, IT, a project manager?)
- What training does the vendor provide? What does Steve's team need to provide?
- How will success be measured at 30/60/90 days?
- What's the backup plan if adoption is low?

**Change management:**
- Which reps will be early adopters? (Start with them)
- What's the incentive to use the tool? (Carrots work better than mandates for AI tools)
- How will Steve communicate the "why" — not "we bought this" but "here's the problem it solves"?

**Contractual:**
- Initial term: 6-12 months max for unproven vendors
- Get exit clauses if adoption falls below agreed metrics
- Data portability: can you export everything if you leave?
- Renewal notice: how many days before the renewal does Steve need to cancel?

---

## ROI Calculation Approach

**Define success metrics before signing:**
1. What specific behavior should change because of this tool?
2. How will that behavior be measured?
3. What's the dollar value of the behavior change?

**Example calculation (hypothetical):**
- Tool: AI-powered call recording and coaching
- Target behavior: Reps improve discovery quality, increasing win rate by 3%
- Team revenue: $5M annual quota
- 3% win rate improvement = $150K additional revenue
- Tool cost: $20K/year for team
- ROI: 7.5x

**Track actual vs. projected ROI at 90 days and 6 months.** If it's not tracking, address it directly — either fix the adoption problem or cancel before the renewal window closes.

---

*Being the manager who evaluates AI tools with rigorous, business-focused criteria — not just "this is cool" — is a Director-level behavior. Use this framework to show up at that level.*
