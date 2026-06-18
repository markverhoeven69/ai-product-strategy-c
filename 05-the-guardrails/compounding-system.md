# Compounding System Design

## Feedback Loops

| Loop                  | Input                                                                                    | Output                                                                   | Compounds? | Status |
| --------------------- | ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | ---------- | ------ |
| Recursive Learning    | User feedback on recommendations, completed goals, rejected suggestions, daily check-ins | Improved recommendation prompts and personalized coaching strategies     | Y          | Active |
| Cross-Domain Transfer | Behavioral insights from exercise, nutrition, sleep and stress coaching domains          | Reusable intervention patterns applied across multiple lifestyle domains | Y          | Active |
| Network Intelligence  | Aggregated and anonymized user behavior data across the platform                         | Population-level insights that improve recommendations for future users  | Y          | Broken |

### Broken Loop Identified by Partner

Network Intelligence is not fully operational because successful and unsuccessful intervention outcomes are not yet systematically aggregated across the entire user base.

### Fix Plan

Implement a centralized behavioral insights pipeline that captures intervention outcomes, identifies high-performing coaching strategies, and feeds these learnings into the recommendation engine on a monthly basis.

---

## Context Connectivity

### How does knowledge flow across teams and domains?

User goals → Coaching Agent → Progress Tracking → Recommendation Engine → Personalized Interventions

User feedback → Analytics Layer → Product Team → Prompt Optimization → Coaching Agent

Behavioral science research → Content Library → Recommendation Engine → User Coaching

### Where does it silo?

Individual coaching conversations generate valuable behavioral insights, but these insights are not yet automatically transferred into product improvement workflows.

Support feedback and user objections are reviewed manually and are not consistently incorporated into coaching strategy updates.

### Live Diagnostic

Loops mapped: 3

Loops that actually compound: 2

Active / Broken / Missing: 2 / 1 / 0


### Freeze Test

If the underlying foundation model remained unchanged for three months, the Lifestyle Companion would still improve because user feedback, behavioral outcomes, and coaching effectiveness data continue to generate proprietary insights that improve future recommendations. The long-term moat is not the LLM itself, but the behavioral intelligence built from user interactions.

---

## Governance Policy

**Scope:**
**Autonomy boundaries:**
**Escalation triggers:**
**Audit cadence:**
**Regulatory exposure (EU AI Act / other):**

## Agent Topology
<!-- If using agents: what can each agent do? What can't it do? Who approves what? -->

## Shadow AI Audit

| Tool | Owner | Risk Level | Decision |
|------|-------|-----------|----------|
| | | H / M / L | keep / govern / kill |
| | | H / M / L | keep / govern / kill |
| | | H / M / L | keep / govern / kill |

**Total tools found:**
**Tools after triage:**
**Estimated hidden spend:**
