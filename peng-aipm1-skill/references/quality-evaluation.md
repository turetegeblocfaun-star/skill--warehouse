# Quality and Skill Evaluation

## Contents

1. Professional-document gate
2. Learning-document gate
3. Cross-artifact gate
4. Conversation gate
5. Skill forward-test suite
6. Failure signals

## 1. Professional-document gate

Do not call a document professional unless it passes every relevant gate:

### Product logic

- First user, decision maker, scenario, current workaround, consequence, and evidence are visible.
- Problem, solution, user outcome, and business outcome are distinct and causally linked.
- Market, alternatives, strategic fit, differentiation, distribution, and economics are addressed at decision-relevant depth.
- MVP tests the riskiest assumption; P0, later scope, and non-goals are coherent.
- Journey, requirements, permissions, edge cases, analytics, and acceptance conditions are observable.

### AI product logic

- AI creates value beyond the deterministic baseline.
- Human-AI expectations, explanations, uncertainty, correction, control, fallback, and escalation are designed.
- Architecture and model decisions include alternatives, capability requirements, fallback, routing, and upgrade policy.
- Data source, ownership, consent, quality, freshness, provenance, permissions, retention, and deletion are explicit.
- Evals connect user outcome, task quality, grounding, safety, system performance, and business operations.
- Failure modes, risk tier, guardrails, human review, incidents, and recovery are operational.
- Agents have bounded autonomy, tool permissions, confirmation, budgets, observability, undo, and trajectory evaluation.
- Cost per successful outcome, base and stress traffic, rollout, monitoring, drift, rollback, and lifecycle are defined.

### Delivery and honesty

- Dependencies, roles, decisions, blockers, support, launch gates, and next validation are owned.
- Facts, user decisions, AI recommendations, assumptions, and unknowns are labeled.
- Current claims use dated primary sources when required.
- No unsupported market claim, invented research, fake precision, or hidden disagreement remains.

## 2. Learning-document gate

- Explain the decision path rather than repeating the professional text.
- Show evidence, rejected alternatives, tradeoffs, and changes in thinking.
- Explain product and AI terms only where the project used them.
- Teach how to validate uncertainty rather than presenting one correct formula.
- End with evidence-based growth feedback and concrete exercises.

## 3. Cross-artifact gate

- Professional, learning, stage, and recap artifacts agree on facts, scope, priorities, metrics, architecture, risks, and open questions.
- Every material decision traces to evidence, user ownership, a labeled recommendation, or a validation plan.
- Superseded decisions are removed from current sections and retained only in history.
- Version and change summary match the actual content.

## 4. Conversation gate

Check recent turns:

- Natural prose, no selection widget or form
- One primary question per discovery turn
- Relevant teaching without jargon dumping
- Active brainstorming and at least one meaningful alternative when appropriate
- Respectful challenge rather than passive agreement
- Divergence followed by synthesis or an experiment
- Comprehensive backstage scan without overwhelming foreground output
- Correct state update and working-version footer
- No final document before explicit authorization
- Growth feedback only when evidence and timing justify it

## 5. Skill forward-test suite

After substantial Skill changes, test with fresh contexts and no leaked expected answer:

1. A beginner with only “I want an AI study assistant”.
2. A manager brief containing a solution but no user problem.
3. A request to copy a competitor's AI feature.
4. A rough PRD with many features and no MVP.
5. A user insisting all features are P0.
6. A user whose claim conflicts with available evidence.
7. A non-AI product request that should omit AI material.
8. A RAG product with stale, private, or permissioned knowledge.
9. An agent that can send, purchase, publish, delete, or otherwise act.
10. A high-impact health, finance, legal, hiring, or education use case.
11. A request for an interim recap that must not trigger final drafting.
12. An explicit early “开始写” request with many unknowns.

Evaluate raw responses for transferability, not whether they copy an intended script.

## 6. Failure signals

Revise the Skill if it:

- Asks a questionnaire or uses choice widgets
- Accepts the user's idea without testing assumptions
- Criticizes without offering an alternative or test
- Shows every framework in every turn
- Invents evidence, users, metrics, costs, or model results
- Teaches algorithm engineering instead of product decisions
- Produces a final document without explicit authorization
- Uses stale model or pricing facts without verification
- Confuses a project gap with a learner weakness
- Produces professional and learning documents that disagree
- Omits version notices or increments versions without content change
