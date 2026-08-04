---
layout: default
---

Denver, CO · Hybrid or remote

Twelve years building enterprise product in brokerage, wealth management, and trading, now focused on AI systems that make decisions people can inspect and act on.

Everything below is deployed and running — not slides. Working retrieval, agentic workflows, decision scoring, structured refusal, and measured evaluation results. Source code and evaluation methodology are public.

Built with Python, LangGraph, ChromaDB, React, and Streamlit, using Claude Code and VS Code.

**On this page:** [Deployed work](#deployed-work) · [Approach](#approach) · [Contact](#contact)

## Deployed work

**[Advisor Transition Risk — Live Demo](https://stevelanderson42.github.io/advisor-transition-risk/)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/advisor-transition-risk)

When a wealth-management advisor leaves, some of their clients leave with them. This models that chain in three stages: which advisors may depart, which households would follow them out, and how much of the book a transition actually recovered.

The core modeling decision is that household departure risk has two independent components — the likelihood a family leaves regardless of advisor, and the likelihood they follow a specific advisor out the door. They're driven by different signals and imply different interventions, so the system scores and displays them separately.

Every score decomposes into its contributing factors inline. Where the data is too thin to score, the system says so and lists which signals are missing and which are present but unreliable — rather than producing a confident-looking number from nothing.

Python scoring engine, React front end, synthetic data. Built and deployed in one day.

**[Agentic Case Triage Workflow — Live Demo](https://ai-case-triage-workflow.streamlit.app)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/agentic-case-triage)

A six-node LangGraph workflow that classifies operational cases, extracts entities, retrieves policy from the RAG layer, scores priority, and produces a routing decision with human-in-the-loop escalation.

Every node's input, output, and rationale is exposed in an execution trace — showing how agentic workflows can be bounded and auditable rather than opaque.

**[RAG Knowledge Pilot — Live Demo](https://rag-knowledge-pilot.streamlit.app)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/rag-knowledge-pilot)

A retrieval system that treats refusal as a first-class output rather than a failure. Evaluated across 15 domain-realistic queries: 90.9% grounded-answer rate and 100% refusal correctness.

The demo shows three behaviors side by side — grounded answer, structured refusal with reason codes, and controlled reflection retry.

**[Requirements Guardrails — Live Demo](https://requirements-guardrails.streamlit.app)** · [Code & README](https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/requirements-guardrails)

A deterministic pre-invocation classifier that decides whether an AI request can safely proceed, routing to PROCEED, CLARIFY, ESCALATE, or BLOCK before any model is called.

Compare Mode runs the classifier with and without its control mechanisms side by side, so the architectural difference is visible rather than asserted.

**[Senior Living Revenue Risk Triage — Rapid Concept Prototype](https://revenue-risk-triage-97zo.bolt.host)**

Built in Bolt to explore revenue-cycle workflows for accounts receivable and claims follow-up. Deterministic rules classify risk; the LLM layer generates explanations, next-best-action guidance, and payer correspondence but never assigns or changes the score.

Mock data and mock AI responses. Built to test how fast a workflow concept can be made tangible.

**[Full portfolio repository →](https://github.com/stevelanderson42/ai-prod-mgr)**

## Approach

Make the behavior inspectable before scaling it. Define the decision boundary, retrieve from approved sources, measure grounding and refusal, log the decision path, and surface uncertainty instead of hiding it.

That discipline comes from a decade of shipping product surfaces in regulated financial services, where every decision a system makes has to be explainable after the fact.

## Contact

[LinkedIn](https://www.linkedin.com/in/steve-l-anderson-1a16391/) · stevelanderson.42@gmail.com · [GitHub](https://github.com/stevelanderson42/ai-prod-mgr)
