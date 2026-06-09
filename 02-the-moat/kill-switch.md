# Kill Switch Audit

## Vendor Dependency Assessment

| Dimension | Current State | Risk Level | 48-Hour Action |
|-----------|--------------|------------|---------------|
| **Provider** | OpenAI is currently the primary reasoning engine for coaching, recommendations and conversational AI. | M | Switch API traffic to Anthropic Claude, Google Gemini or Azure OpenAI using predefined provider adapters. |
| **Abstraction** | AI functionality is designed behind an application service layer rather than being embedded directly into business logic. | M | Redirect model calls through a provider-agnostic interface and update provider configuration without changing core workflows. |
| **Routing** | Single-provider routing initially, with future support for multi-model routing based on use case and cost. | H | Single-provider routing initially, with future support for multi-model routing based on use case and cost. |
| **Eval** | Human review and user feedback provide quality validation. Automated evaluation benchmarks are planned but not yet implemented. | H | Run predefined regression tests and compare output quality across alternative providers before full migration. |

## Portability Score
### Partial
The product is intentionally designed to keep behavioural data, coaching outcomes, user profiles and healthcare workflows outside the foundation model. However, the current prototype relies primarily on a single AI provider and lacks automated model-routing and evaluation capabilities.

## If OpenAI doubles pricing tomorrow:

Within 48 hours, The AI Lifestyle Companion would:

1. Freeze non-essential AI features.
2. Activate a secondary provider (Anthropic, Gemini or Azure OpenAI).
3. Redirect conversational workloads through a provider abstraction layer.
4. Maintain access to all behavioural data, coaching history and user profiles because these are stored in platform-controlled infrastructure.
5. Continue delivering core coaching workflows with limited user impact.

The business remains operational because the AI model is treated as a replaceable reasoning component rather than the system of record.

## If OpenAI ships a competing product:
A generic AI lifestyle coach could replicate conversations, recommendations and habit-tracking features.

What remains defensible is:

* Proprietary behavioural outcome data.
* Longitudinal lifestyle improvement datasets.
* Integration with Dutch healthcare organisations.
* Access to certified lifestyle coaches.
* Knowledge of reimbursement pathways and preventive healthcare programmes.
* Evidence-based intervention effectiveness across user segments.
* A workflow connecting users, AI coaching, human coaching and measurable health outcomes.

The long-term moat is not AI coaching itself, but becoming embedded within the Dutch preventive healthcare ecosystem where data, workflows, coaches and healthcare partners create value that a general-purpose AI assistant cannot easily replicate.
