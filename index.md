---
layout: default
---

<section class="hero">
  <div class="eyebrow">Denver, CO · Hybrid or remote · Actively interviewing</div>

  <h1>Senior Product Manager building governed AI workflows for regulated domains</h1>

  <p class="hero-subtitle">
    I build inspectable AI product prototypes that combine product judgment, governed retrieval,
    structured refusal, agentic workflow orchestration, and audit-ready execution traces.
  </p>

  <p class="hero-context">
    12+ years in regulated financial services across banking, wealth management, trading, APIs,
    SaaS integrations, Agile delivery, and enterprise platform modernization.
  </p>

  <div class="hero-actions">
    <a class="button primary" href="#core-ai-product-modules">View AI Modules</a>
    <a class="button secondary" href="https://github.com/stevelanderson42/ai-prod-mgr">GitHub Portfolio</a>
    <a class="button secondary" href="https://www.linkedin.com/in/steve-l-anderson-1a16391/">LinkedIn</a>
  </div>
</section>

<section class="proof-strip">
  <div>
    <strong>RAG</strong>
    <span>Grounded retrieval + structured refusal</span>
  </div>
  <div>
    <strong>Agents</strong>
    <span>LangGraph case triage + execution traces</span>
  </div>
  <div>
    <strong>Governance</strong>
    <span>Policy boundaries before model calls</span>
  </div>
  <div>
    <strong>PM Judgment</strong>
    <span>Workflow, risk, evaluation, escalation</span>
  </div>
</section>

<nav class="page-nav">
  <a href="#core-ai-product-modules">Core AI Modules</a>
  <a href="#rapid-prototyping">Rapid Prototype</a>
  <a href="#product-approach">Product Approach</a>
  <a href="#contact">Contact</a>
</nav>

<section id="core-ai-product-modules">
  <h2>Core AI Product Modules</h2>

  <p class="section-intro">
    These modules are deployed, inspectable, and designed to show how AI behavior can be bounded,
    measured, and explained before scaling into high-stakes enterprise workflows.
  </p>

  <div class="project-grid">

    <article class="project-card featured">
      <div class="project-label">Governance Boundary</div>
      <h3>Requirements Guardrails</h3>

      <p>
        A deterministic pre-invocation classifier that decides whether an AI request can safely proceed —
        routing to <strong>PROCEED</strong>, <strong>CLARIFY</strong>, <strong>ESCALATE</strong>, or
        <strong>BLOCK</strong> before any model is called.
      </p>

      <div class="tags">
        <span>Pre-invocation control</span>
        <span>Deterministic routing</span>
        <span>Audit trail</span>
        <span>Governance</span>
      </div>

      <div class="card-actions">
        <a href="https://requirements-guardrails.streamlit.app">Live Demo</a>
        <a href="https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/requirements-guardrails">Code & README</a>
      </div>
    </article>

    <article class="project-card">
      <div class="project-label">Retrieval + Evaluation</div>
      <h3>RAG Knowledge Pilot</h3>

      <p>
        A measured retrieval system that treats refusal as a first-class product behavior, not an error.
      </p>

      <div class="metric-row">
        <div>
          <strong>90.9%</strong>
          <span>grounded answer rate</span>
        </div>
        <div>
          <strong>100%</strong>
          <span>refusal correctness</span>
        </div>
      </div>

      <p>
        Evaluated on 15 domain-realistic compliance queries. The demo shows grounded answers,
        structured refusals with reason codes, and controlled reflection retry.
      </p>

      <div class="tags">
        <span>RAG</span>
        <span>Groundedness</span>
        <span>Refusal logic</span>
        <span>Evaluation</span>
      </div>

      <div class="card-actions">
        <a href="https://rag-knowledge-pilot.streamlit.app">Live Demo</a>
        <a href="https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/rag-knowledge-pilot">Code & README</a>
      </div>
    </article>

    <article class="project-card">
      <div class="project-label">Agentic Workflow</div>
      <h3>Agentic Case Triage Workflow</h3>

      <p>
        A six-node LangGraph workflow that classifies operational cases, extracts entities, retrieves policy
        from the RAG layer, scores priority, drafts routing notes, and produces a final routing decision.
      </p>

      <p>
        Every node's input, output, and rationale are exposed in an execution trace.
      </p>

      <div class="tags">
        <span>LangGraph</span>
        <span>Case triage</span>
        <span>Human escalation</span>
        <span>Execution trace</span>
      </div>

      <div class="card-actions">
        <a href="https://ai-case-triage-workflow.streamlit.app">Live Demo</a>
        <a href="https://github.com/stevelanderson42/ai-prod-mgr/tree/main/modules/agentic-case-triage">Code & README</a>
      </div>
    </article>

  </div>

  <p class="repo-link">
    <a href="https://github.com/stevelanderson42/ai-prod-mgr">View full AI Product Manager portfolio repository →</a>
  </p>
</section>

<section id="rapid-prototyping">
  <h2>Rapid Prototyping</h2>

  <article class="prototype-card">
    <div>
      <div class="project-label">Bolt Rapid Prototype</div>
      <h3>Senior Living Revenue Risk Triage</h3>

      <p>
        A rapid prototype built in Bolt to explore senior-living revenue-cycle workflows for accounts
        receivable and claims follow-up. The prototype uses mock account data and deterministic rules to
        classify risk based on days outstanding, claim denial status, eligibility, and authorization state.
      </p>

      <p>
        The LLM layer is intentionally bounded: it generates plain-language explanations, next-best-action
        guidance, payer correspondence, and audit-style notes from structured account data — but it does not
        assign or change the risk score.
      </p>

      <div class="tags">
        <span>Revenue cycle</span>
        <span>Workflow decomposition</span>
        <span>Rules + LLM boundary</span>
        <span>Mock data</span>
      </div>
    </div>

    <div class="prototype-side">
      <p>
        Built to demonstrate rapid AI-assisted prototyping and a practical boundary between deterministic
        scoring and LLM-generated operational support.
      </p>
      <a class="button primary" href="https://revenue-risk-triage-97zo.bolt.host">View Prototype</a>
    </div>
  </article>
</section>

<section id="product-approach">
  <h2>Product Approach</h2>

  <div class="approach-grid">
    <div class="approach-card">
      <h3>1. Define the boundary</h3>
      <p>Define what the AI system may do, must refuse, and should escalate.</p>
    </div>

    <div class="approach-card">
      <h3>2. Retrieve from approved sources</h3>
      <p>Keep high-stakes answers grounded in known policy and approved reference material.</p>
    </div>

    <div class="approach-card">
      <h3>3. Measure behavior</h3>
      <p>Treat groundedness, refusal correctness, and escalation as product requirements.</p>
    </div>

    <div class="approach-card">
      <h3>4. Make decisions inspectable</h3>
      <p>Expose the execution path, rationale, retrieved context, and failure modes.</p>
    </div>
  </div>

  <p class="closing-note">
    This is the discipline I bring from regulated financial-services product work into LLM and agentic systems —
    informed by years of building product surfaces and customer-facing disclosures adjacent to model risk governance.
  </p>
</section>

<section id="contact" class="contact-section">
  <h2>Contact</h2>

  <p>
    <a href="https://www.linkedin.com/in/steve-l-anderson-1a16391/">LinkedIn</a>
    <span>·</span>
    <a href="mailto:stevelanderson.42@gmail.com">stevelanderson.42@gmail.com</a>
    <span>·</span>
    <a href="https://github.com/stevelanderson42/ai-prod-mgr">GitHub</a>
  </p>
</section>