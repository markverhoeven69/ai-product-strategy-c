# Cost Curve & Pricing Strategy

## Cost Model

| Cost Category | Per-User/Month | Notes |
|--------------|----------------|-------|
| Inference (primary model) | €1.20 | Daily coaching conversations, habit recommendations |
| Inference (cascading/triage) | €0.40 | Small model handles ~80% of requests |
| Infrastructure | €0.50 | Hosting, API gateway, monitoring |
| Data/storage | €0.20 | User profiles, history, embeddings |
| Human-in-the-loop | €0.30 | Occasional review of edge cases and safety checks |
| **Total AI COGS** | €2.60 | Blended monthly AI cost |

## Cascading Strategy

**Triage model:** 
GPT-4.1 Mini / Claude Haiku equivalent

**Frontier model:**
GPT-4o / Claude Sonnet equivalent

**Routing rule:**
* Habit reminders
* Goal tracking
* FAQ questions
* Progress summaries
  
→ Frontier model

* Personalized lifestyle plans
* Multi-step coaching
* Emotional support conversations
* Complex health reasoning
  
→ Frontier model

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
* Meal suggestions
* Sleep insights
* Progress reports

These cost little but improve retention and ARPU.

### Killers
Keep as premium add-ons:

* Deep agentic health planning
* Long-form report generation
* Continuous monitoring workflows
* Image-based nutrition analysis
* Integration with wearables and automated coaching loops

These create disproportionate inference costs and should not be bundled into the base plan.

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

**Proposed AI pricing:**

***Essential***
€12.99/month

Includes:

* AI coach
* Daily guidance
* Goal tracking
* Weekly summaries

***AI Coach Pro***
€24.99/month

Includes:

* Unlimited coaching
* Advanced plans
* Predictive insights
* Premium AI models

***AI Health Agent***
€49.99/month

Includes:

* Deep analysis
* Multi-step planning
* Wearable integrations
* Autonomous coaching workflows


**Model:**

***Hybrid***

* Base subscription (seat-based)
* Premium AI usage tiers
* Outcome-oriented value proposition

Goal: move toward outcome pricing rather than pure access pricing.

## Stress Tests

| Scenario | Impact on Margin | Response |
|----------|-----------------|----------|
| Inference costs 3x | Margin drops from ~80% to ~60% | Increase routing to small model, tighten prompts |
| Heaviest segment doubles | AI COGS increase ~40% | Introduce usage limits and premium tier |
| Model provider raises prices 50% | Margin drops ~10–15 pts | Multi-provider strategy and renegotiate contracts |

## Board One-Pager

**Before (traditional SaaS):**
* Revenue/User/Month: €9.99
* COGS/User/Month: €0.80
* Gross Margin: ~92%
* Value proposition:

Static lifestyle app with limited personalization.

**After (AI-enabled):**
* Revenue/User/Month: €24.99
* COGS/User/Month: €2.60
* Gross Margin: ~90%
* Value proposition:

Personal AI lifestyle coach delivering personalized guidance, recommendations, and behavior-change support at scale.

**Net margin shift:**
* Revenue increase: +150%
* AI cost increase: +225%

Net result:

* Significantly higher customer value
* Higher retention
* Stronger differentiation
* Sustainable margins through cascading architecture

### Narrative for the Board
We intentionally accept higher variable AI costs because AI transforms the product from a static wellness app into a personalized lifestyle coach. Cascading architecture keeps costs predictable while premium outcome-based pricing captures the additional value created.
