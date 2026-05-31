---
layout: default
---

*Denver, CO · Hybrid or remote · Actively interviewing for senior AI Product Manager roles*

I'm a senior product manager with 12+ years in regulated financial services, now focused on governed AI workflows for banking, wealth management, and trading contexts.

This portfolio is deployed and inspectable — working RAG retrieval, agentic case triage, structured refusal, audit-ready execution traces, live demos, and measured evaluation results.

Built across the modern AI product prototyping stack — deeper deployed modules built with Python, Streamlit, LangGraph, VS Code, and Claude Code; rapid concept prototypes built with tools like Bolt.

**On this page:** [Core AI modules](#core-ai-product-modules) · [Rapid Bolt prototype](#rapid-prototyping) · [Product approach](#product-approach) · [Contact](#contact)

## Core AI product modules

**[Requirements Guardrails — Live Demo](https://requirements-guardrails.streamlit.app)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/requirements-guardrails)

A deterministic pre-invocation classifier that decides whether an AI request can safely proceed — routing to PROCEED, CLARIFY, ESCALATE, or BLOCK before any model is called.

The live demo includes a Compare Mode: one toggle runs the classifier with and without its governance mechanisms, side by side, so you can see exactly how the architecture changes the outcome. No general-purpose LLM sits at the decision boundary — every classification traces to a rule or a documented mechanism, with a full audit trail.

**[RAG Knowledge Pilot — Live Demo](https://rag-knowledge-pilot.streamlit.app)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/rag-knowledge-pilot)

A measured retrieval system that treats refusal as a first-class output, not an error.

Evaluated on 15 domain-realistic compliance queries: 90.9% grounded answer rate at the higher threshold with reflection, and 100% refusal correctness.

The live demo shows three governed behaviors — grounded answer, structured refusal with reason codes, and controlled reflection retry.

**[Agentic Case Triage Workflow — Live Demo](https://ai-case-triage-workflow.streamlit.app)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/agentic-case-triage)

A six-node LangGraph workflow that classifies operational cases, extracts entities, retrieves policy from the RAG layer, scores priority, drafts internal routing notes, and produces a final routing decision.

Every node's input, output, and rationale are exposed in an execution trace — showing how agentic workflows can be bounded, auditable, and integrated with governed retrieval.

**[Full portfolio repository →](https://github.com/stevelanderson42/ai-prod-mgr)**

## Rapid prototyping

**[Revenue Risk Triage — Bolt Rapid Prototype](https://revenue-risk-triage-97zo.bolt.host)**

A rapid prototype built in Bolt to explore senior-living revenue-cycle workflows for accounts receivable and claims follow-up. The prototype uses mock account data and deterministic rules to classify risk based on days outstanding, claim denial status, eligibility, and authorization state.

The LLM layer is intentionally bounded: it generates plain-language explanations, next-best-action guidance, payer correspondence, and audit-style notes from structured account data — but it does not assign or change the risk score.

*Built to demonstrate rapid AI-assisted prototyping, workflow decomposition, and a practical boundary between rules-based decisions and LLM-generated operational support. Public demo uses mock data and mock AI responses; no live API key is exposed.*

## Product approach

My approach is to make AI behavior inspectable before it is scaled — define the policy boundary, retrieve from approved sources, measure grounding and refusal behavior, log the decision path, and escalate uncertainty instead of hiding it.

That is the discipline I bring from regulated FinServ product work into LLM and agentic systems — informed by years of building product surfaces and customer-facing disclosures adjacent to model risk governance (SR 11-7), across credit, fraud, suitability, AML, and vendor models.

## Contact

[LinkedIn](https://www.linkedin.com/in/steve-l-anderson-1a16391/) · stevelanderson.42@gmail.com · [GitHub](https://github.com/stevelanderson42/ai-prod-mgr)