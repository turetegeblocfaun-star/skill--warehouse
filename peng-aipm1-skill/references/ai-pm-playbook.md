# AI Product Manager Playbook

## Contents

1. AI PM boundary
2. AI suitability and task definition
3. Human-AI experience
4. System and model strategy
5. Data and knowledge strategy
6. Evaluation system
7. Safety, governance, and human review
8. Agent autonomy and actions
9. Economics, delivery, and lifecycle
10. Current-fact research

## 1. AI PM boundary

Own the product decisions that translate probabilistic capability into user value, measurable behavior, controlled failure, and sustainable operation.

Go deep enough to define requirements, compare alternatives, question engineering, set evals, and accept risk. Avoid training mathematics, model implementation, distributed systems code, GPU operations, and infrastructure recipes unless they change a product decision.

## 2. AI suitability and task definition

Before choosing AI, define:

- User task, product surface, input, output, decision, and consequence
- Current human, rule-based, search, workflow, or traditional-ML baseline
- Unique value created by generation, retrieval, prediction, perception, adaptation, or tool use
- Acceptable variability and cost of a wrong, missing, delayed, or refused result
- What remains deterministic for permissions, billing, compliance, calculations, and auditability
- What the user can inspect, edit, confirm, undo, or escalate

Reject AI when a simpler system meets the outcome more reliably and economically. Reject “competitors have AI” as the only rationale.

## 3. Human-AI experience

Design how users understand and control the system:

- Set realistic expectations before first use
- Explain benefit and boundary without exposing unnecessary technical detail
- Provide examples of suitable and unsuitable tasks
- Show sources, uncertainty, confidence, or rationale only when they improve decisions
- Let users edit, correct, regenerate, compare, undo, and provide structured feedback
- Distinguish suggestion, draft, recommendation, and executed action
- Provide graceful deterministic fallback and human escalation
- Avoid anthropomorphic cues that overstate understanding or authority
- Measure automation bias, over-trust, correction burden, and abandonment

## 4. System and model strategy

Compare the simplest viable pattern:

| Pattern | Prefer when | Product risk |
|---|---|---|
| Prompt only | General knowledge and short context are enough | Inconsistent or stale behavior |
| Few-shot | Examples stabilize style, labels, or structure | Example bias and brittleness |
| RAG | Private, fresh, permissioned, or citable knowledge is required | Retrieval quality, access, and provenance |
| Fine-tune | Repeated behavior or domain pattern resists prompting and data exists | Data quality, lock-in, drift, retraining |
| Agent | The system must plan and use tools across multiple steps | Compounding errors, permissions, cost, observability |
| Hybrid | Different steps require different controls | Complexity and operational burden |

Define capability criteria before a vendor name. Specify primary, fallback, routing, outage behavior, degraded mode, context limits, latency, cost, version pinning, upgrade evaluation, build-versus-buy, portability, and vendor exit risk.

## 5. Data and knowledge strategy

Cover:

- Source, owner, license, consent, representativeness, and allowed purpose
- Collection, cleaning, labeling, quality, coverage, freshness, and provenance
- Tenant, document, row, and field permissions
- Retrieval chunking, indexing, recall, reranking, citation mapping, and stale-source handling at product-requirement depth
- Sensitive data, minimization, retention, deletion, residency, and audit
- User feedback meaning, incentives, noise, abuse, privacy, and contamination
- Data flywheel hypothesis and conditions under which it fails
- Training or vendor-use restrictions

Do not call data a moat without explaining exclusive access, quality, feedback, and compounding advantage.

## 6. Evaluation system

Treat the eval suite as part of the product specification.

Define six layers:

1. **User outcome:** Does the user finish the real task better, faster, or more safely?
2. **Task quality:** Does the output meet a project-specific rubric?
3. **Grounding and retrieval:** Are sources relevant, allowed, fresh, and correctly cited?
4. **Safety and refusal:** Does the system refuse harmful tasks without blocking normal use?
5. **System performance:** Latency, availability, tool success, recovery, and observability.
6. **Business and operations:** Cost per successful outcome, adoption, retention, support, and human-review burden.

Build a versioned golden set with normal, difficult, ambiguous, edge, adversarial, multilingual, segment-specific, and production-incident cases. Record source, expected behavior or rubric, owner, disagreement process, and update cadence.

Use deterministic checks where possible, expert human evaluation where judgment matters, pairwise comparison for relative quality, model graders only after calibration, and online metrics for real behavior. Define thresholds, confidence, sample size assumptions, stop conditions, and regression policy. Add production failures back into the suite.

Never use “accurate”, “smart”, “helpful”, or “safe” without an observable test. Never claim 100% quality for a hard generative task because a small set passed.

## 7. Safety, governance, and human review

Set risk proportionate to consequence, reversibility, affected population, scale, and autonomy.

Layer controls across input, context, model, output, action, human review, and incident response. Cover prompt injection, data exfiltration, unsupported claims, stale or unauthorized retrieval, bias, harmful advice, impersonation, misuse, over-refusal, privacy, abuse, outage, cost runaway, and drift.

For health, finance, legal, employment, education access, public safety, or other consequential decisions, require qualified human review for high-impact actions and specialist compliance assessment. Do not present the product document as legal approval.

Make human review operational: define reviewer expertise, queue, SLA, workload, cost, override, appeal, escalation, audit trail, and fallback when the queue fails.

## 8. Agent autonomy and actions

Choose the minimum necessary autonomy:

1. Explain or recommend
2. Draft an action
3. Prepare and wait for confirmation
4. Execute a narrow reversible action
5. Execute bounded multi-step work
6. Operate autonomously within explicit policy

For every tool or action, define purpose, user identity, least privilege, allowed resources, argument constraints, spend/rate/time limits, confirmation, idempotency, observable result, undo, partial failure, escalation, and audit.

Evaluate full trajectories, not only individual outputs. Monitor whether a sequence continues to serve the user's intent and whether safeguards can pause, inspect, and roll back the run.

## 9. Economics, delivery, and lifecycle

Model calls per task, context and output tokens, retrieval, embeddings, reranking, tool costs, retries, evals, observability, storage, support, and human review. Track cost per successful outcome, not only cost per call. Model base, 10×, and stress scenarios.

Connect cost to pricing, value, gross margin, limits, caching, routing, quality tiers, adoption, and abuse. Include acquisition, onboarding, distribution, willingness to pay, procurement, support, and vendor dependence.

Deploy through offline eval, shadow traffic, internal use, canary, percentage rollout, and general availability. Define entry, observation, stop, rollback, and owner at every stage. Version model, prompt, retrieval, policy, tool, data, and eval set. Monitor segment drift, incidents, quality, latency, cost, and human workload.

## 10. Current-fact research

When a decision depends on current model capability, price, limit, regulation, provider policy, competitor, or market fact:

1. Research current primary or official sources.
2. Record access date and exact source.
3. Separate direct fact from inference.
4. Avoid long quotations and unsupported comparisons.
5. Recheck before launch or procurement.
6. Prefer capability requirements that survive a model or vendor swap.
