# Cost Curve & Pricing Strategy

## Cost Model

| Cost Category | Per-User/Month | Notes |
|--------------|----------------|-------|
| Inference (primary model) | €0.25 | Daily coaching conversations, habit recommendations |
| Inference (cascading/triage) | €0.20 | Small model handles ~80% of requests |
| Infrastructure | €0.50 | Hosting, API gateway, monitoring |
| Data/storage | €0.20 | User profiles, history, embeddings |
| Human-in-the-loop | €0.20 | Occasional review of edge cases and safety checks |
| **Total AI COGS** | €1.35 | Blended monthly AI cost |

**Assumption:** 150 AI interactions per active user per month, with 80% routed to a low-cost model and 20% routed to a frontier model.

### Input Margin Calculator

| Input                          | Waarde     | Toelichting                          |
| ------------------------------ | ---------- | ------------------------------------ |
| Avg AI Requests / User / Month | 150    | 3-5 interacties per dag              |
| Blended Cost per Request       | $0.003 | 80% mini-model, 20% frontier-model   |
| Revenue per User / Month       | $19.99 | Premium AI coaching subscription     |
| Non-AI COGS / User / Month     | $2.00  | Hosting, support, analytics, storage |


## Cascading Strategy

**Triage model:** 
GPT-4.1 Mini / Claude Haiku equivalent

**Frontier model:**
GPT-4o / Claude Sonnet equivalent

**Routing rule:**

→ Small model

* Habit reminders
* Goal tracking
* FAQ questions
* Progress summaries
  
→ Frontier model

* Personalized lifestyle plans
* Multi-step coaching
* Emotional support conversations
* Health information synthesis and long-context reasoning

**Expected cascade ratio:**
* 80% Small model
* 20% Frontier model

Most traffic should hit the cheap model while only complex requests go to the expensive layer.

## Bundling Strategy (Leaders, Fillers & Killers)

### Leader
Features users primarily come for:

* AI Lifestyle Coach
* Personalized daily recommendations
* Goal-based action plans

These are the core value drivers and justify subscription pricing.

### Fillers
Low-cost features that increase perceived value:

* Daily summaries
* Motivational messages
* Habit streak tracking
* Sleep insights
* Progress reports

These cost little but improve retention and ARPU.

### Killers
Keep as premium add-ons:

* Deep agentic health planning
* Long-form report generation
* Continuous monitoring workflows
* Image-based nutrition analysis
* Personalized nutrition planning
* Integration with wearables and automated coaching loops

These create disproportionate inference costs and should not be bundled into the base plan.

Killer usage estimate: 15–25%
Decision: Sell as premium add-on

### 70% Rule
Bundle if >70% of users use it:

#### Bundle
* Daily coach chat
* Progress summaries
* Goal tracking
* Recommendations

#### Premium Add-on
* Advanced health reports
* Wearable integrations
* AI health agent
* Deep analysis workflows

## Pricing Model

**Current pricing:**
€9.99/month premium subscription

### Proposed AI Pricing

#### Essential — €12.99/month

Includes:

* AI lifestyle coach
* Daily guidance and check-ins
* Goal tracking
* Weekly summaries
* Habit and progress insights

Target user:
Users seeking ongoing lifestyle support and accountability.

---

#### AI Coach Pro — €19.99/month

Includes everything in Essential, plus:

* Extended coaching conversations
* Personalized action plans
* Predictive insights and recommendations
* Priority access to frontier AI models

Target user:
Users actively working toward health, fitness, sleep, or productivity goals.

---

#### AI Health Agent — €34.99/month

Includes everything in Pro, plus:

* Deep analysis workflows
* Personalized nutrition planning
* Wearable integrations
* Continuous monitoring and coaching loops
* Autonomous planning and follow-up actions

Target user:
Power users seeking highly personalized and proactive coaching.

---

**Model: Hybrid Subscription**

Primary Revenue Model:

* Seat-based subscription

Secondary Revenue Model:

* Usage-based access for premium AI workflows
* Premium AI Health Agent tier

Future Opportunities:

* Outcome-based coaching programs
* Goal-specific transformation packages
* Partner-sponsored health interventions

### Pricing Philosophy

The core coaching experience remains subscription-based, while high-cost AI workflows are monetized through premium tiers. This aligns customer value with AI consumption and protects long-term margins.

**Goal:** Move toward outcome-oriented pricing while maintaining predictable subscription revenue and sustainable AI economics.

## Stress Tests

| Scenario | Impact on Margin | Response |
|----------|-----------------|----------|
| Inference costs 3x | Margin drops from 88% → 79% | Increase routing to small model, tighten prompts |
| Heaviest segment doubles | Margin drops from 88% → 84% | Introduce usage limits and premium tier |
| Model provider raises prices 50% | Margin drops from 88% → 84% | Multi-provider strategy and renegotiate contracts |

## Board One-Pager

**Before (traditional Lifestyle App):**
* Revenue/User/Month: €9.99
* COGS/User/Month: €0.80
* Gross Margin: ~92%
* Value proposition:

Static habit tracking and lifestyle content.

**After (AI-enabled):**
* Revenue/User/Month: €19.99
* COGS/User/Month: €1.35
* Gross Margin: ~93%
* Value proposition:

Personalized AI coaching and behavior-change support.

**Net margin shift:**
* Revenue increase: +100%
* AI cost increase: +225%

AI costs introduced but remain a small fraction of revenue due to cascading architecture.

Net result:

* Significantly higher customer value
* Higher retention
* Stronger differentiation
* Sustainable margins through cascading architecture

### Narrative for the Board
We intentionally accept higher variable AI costs because AI transforms the product from a static wellness app into a personalized lifestyle coach. Cascading architecture keeps costs predictable while premium outcome-based pricing captures the additional value created.
