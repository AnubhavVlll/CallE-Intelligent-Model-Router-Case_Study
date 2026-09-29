# CallE — Intelligent Model Router

> **Reducing enterprise GenAI operating cost without sacrificing support quality or safety.**

## Overview

CallE is a **B2B customer-support SaaS** case study exploring whether different customer-support interactions should be handled by different AI model capabilities.

The scenario assumes **100,000 AI interactions per month**, with every request currently routed to a premium LLM.

The product question is:

> **Can CallE reduce AI Cost per Resolved Interaction while maintaining quality at or above the premium-model baseline?**

Rather than treating this as simply an LLM comparison exercise, the case study approaches it as an **AI Product Management + Project Management problem** involving business economics, product strategy, model evaluation, safety, architecture, delivery, and governance.

## My Role

**Hybrid AI Product Manager + AI Project Manager**

I focused on:

- Problem framing and product strategy
- Model-routing decision criteria
- Quality and safety thresholds
- AI evaluation framework
- MVP definition and prioritisation
- Routing policy and guardrails
- Human-in-the-loop design
- Technical architecture
- Experiment and pilot design
- Project planning and delivery
- Risk and dependency management
- Stakeholder management
- Business KPI design

Engineering and ML/AI teams are treated as responsible for implementation and model optimisation rather than claiming that I personally built every technical component.

## Proposed Solution

The proposed architecture uses a hybrid routing approach:

```text
Customer Request
       ↓
Risk Assessment
       ↓
Intent / Complexity / Context
       ↓
Routing Policy
       ↓
┌───────────┬───────────┬───────────┐
↓           ↓           ↓
Lower-cost  Mid-tier    Premium
Model       Model       Model
└───────────┴───────────┴───────────┘
       ↓
Response Validation
       ↓
   ┌───┴────┐
   ↓        ↓
 Pass     Failure
   ↓        ↓
Customer  Premium Fallback
              ↓
        Human Escalation
```

High-risk or uncertain requests can bypass normal cost optimisation and be escalated to human support.

## Key Product Decisions

- Optimise **AI Cost per Resolved Interaction**, not simply cost per request.
- Keep the premium model as the quality baseline.
- Use risk as a hard routing constraint.
- Reserve expensive models for requests that genuinely require them.
- Validate responses before automated delivery.
- Use premium fallback when a lower-cost model fails safely.
- Escalate high-risk or unresolved cases to humans.
- Improve the human handoff with structured issue summaries and context.
- Avoid building new RAG infrastructure during the MVP.
- Validate the business hypothesis through a controlled pilot before scaling.

## Evaluation Framework

Candidate models are evaluated across:

| Dimension | Weight |
|---|---:|
| Answer quality | 30% |
| Cost | 25% |
| Latency | 15% |
| Reliability | 10% |
| Context capability | 10% |
| Privacy / security | 10% |

The weights are **product decisions for this hypothetical case**, not universal industry standards.

The evaluation also separates:

- Model quality
- AI safety
- Product performance
- Business performance

## Experiment

### Hypothesis

> If lower-risk and lower-complexity interactions can be routed to appropriately capable lower-cost models while premium capability is reserved for requests that require it, CallE can reduce AI Cost per Resolved Interaction without reducing quality below the premium baseline.

### Control

100% premium-model workflow.

### Treatment

Risk-aware dynamic routing with validation, fallback, and human escalation.

### Primary KPI

**AI Cost per Resolved Interaction**

### Quality Guardrail

Treatment quality must remain at or above the premium baseline.

### Safety Guardrail

No critical safety threshold breach.

## Project Delivery

The proposed MVP/pilot is planned over **12–16 weeks** covering:

1. Discovery and baseline
2. Model evaluation
3. Routing prototype
4. Validation and fallback
5. Support-agent workflow
6. Security and UAT
7. Controlled pilot
8. Executive scale / iterate / stop decision

## Risk Areas

Key risks include:

- Complex requests being routed to insufficient models
- Quality falling below baseline
- Vendor/API dependency
- Insufficient cost savings
- Hallucination
- PII leakage
- Prompt injection
- Model drift
- Excessive fallback
- Scope creep

## Case Study Contents

The full case study covers:

- Business context
- Problem discovery
- User and stakeholder analysis
- Current and future-state journeys
- AI opportunity mapping
- Product vision and strategy
- MVP and prioritisation
- Product requirements
- AI architecture
- Technology decision
- Model evaluation
- Experiment design
- Business economics
- Project charter
- WBS
- Sprint plan
- RACI
- Dependency register
- Risk register
- Stakeholder management
- Change management
- Launch plan
- Governance
- Post-launch monitoring
- Retrospective

## Evidence & Disclosure

This is a **simulated case study**.

The case study does not claim real:

- CallE customers
- User interviews
- Production deployments
- AI performance
- Cost savings
- ROI
- Financial results
- Benchmark results

Illustrative numbers and scenarios are explicitly identified as assumptions or simulations.

The purpose of the project is to demonstrate how an AI Product / Project Manager would structure and evaluate an enterprise AI initiative.

## Files

- `CallE_Intelligent_Model_Router_Case_Study.md` — Full case study

## Core Takeaway

> **AI optimisation is not simply about minimising model cost. It is about maximising business value under quality, safety, operational, and cost constraints.**
