# Complete Product Lifecycle Playbook

## Contents

1. Backstage completeness scan
2. Phase map and gates
3. Milestone artifacts
4. Ordinary-product adaptation

## 1. Backstage completeness scan

Scan these lenses before deciding what to surface:

- Business context, strategy, timing, and decision owner
- End user, buyer, administrator, operator, reviewer, support team, and affected non-user
- Triggering moment, environment, frequency, severity, current workaround, and switching cost
- Functional, emotional, social, accessibility, and trust needs
- Direct competitors, indirect substitutes, manual alternatives, and doing nothing
- Evidence strength, missing evidence, assumptions, contradictions, and reversibility
- User outcome, business outcome, leading indicator, lagging indicator, guardrail metric, and data source
- Value proposition, differentiation, distribution, pricing, unit economics, and defensibility
- Journey, information architecture, interaction, empty state, error, recovery, accessibility, and localization
- MVP, P0/P1/P2, non-goals, dependencies, feasibility, and opportunity cost
- Functional requirements, non-functional requirements, permissions, acceptance conditions, and analytics
- Data, AI, safety, compliance, operations, customer support, launch, incidents, rollback, and iteration

Do not expose the full list each turn. Surface the lenses that change the current decision.

## 2. Phase map and gates

### Phase 0: Intake and orientation

Clarify the request, starting path, intended outcome, decision owner, known constraints, and current evidence.

Gate: state a provisional product sentence and the next uncertainty without inventing facts.

### Phase 1: Opportunity and problem

Define why now, who is affected, the concrete moment, current workaround, consequence, frequency, severity, and evidence.

Gate: distinguish a real or testable problem from a preferred solution.

### Phase 2: Users, stakeholders, and scenarios

Map the first user, buyer, operator, reviewer, administrator, support team, and affected parties. Prioritize a primary scenario and critical secondary scenarios.

Gate: identify the first target segment and primary job without treating “everyone” as a segment.

### Phase 3: Market, business, and strategy

Compare alternatives, distribution, differentiation, willingness to switch or pay, strategic fit, expected value, operating burden, and defensibility.

Gate: explain why this product is worth testing and what would make it unattractive.

### Phase 4: Outcomes, metrics, and validation

Connect product output to behavior change, user outcome, and business outcome. Define baselines, targets, measurement source, observation period, and guardrails.

Gate: define the riskiest assumption and a test that could disprove it.

### Phase 5: Value proposition, MVP, and scope

Define the smallest valuable end-to-end loop, P0/P1/P2, non-goals, rejected alternatives, and the decision rule for expansion.

Gate: every P0 item supports the primary loop or a launch-critical control.

### Phase 6: Journey, experience, and requirements

Map trigger, entry, input, system response, user decision, correction, outcome, repeat use, error, recovery, permission, accessibility, and analytics. Turn the journey into testable requirements.

Gate: a designer, engineer, tester, and operator can observe what “done” means.

### Phase 7: AI product design

Run the full AI PM playbook: AI fit, human-AI UX, system pattern, model strategy, data, evals, safety, agent autonomy, cost, and operations.

Gate: quality is statistically specified, failure is recoverable, and launch thresholds and owners exist.

### Phase 8: Delivery and collaboration

Define roles, decision rights, dependencies, prototype review, technical spike, data preparation, acceptance, test plan, analytics, support readiness, and schedule risk.

Gate: every critical dependency and launch blocker has an owner and decision date.

### Phase 9: Launch and operation

Plan shadow traffic, internal use, canary, percentage rollout, communications, onboarding, support, monitoring, incident severity, pause, rollback, and escalation.

Gate: entry, stop, rollback, and decision criteria are written before exposure.

### Phase 10: Post-launch learning

Compare results with hypotheses, inspect segments and failures, update evals from incidents, review costs and human workload, decide continue/change/stop, and revise the roadmap.

Gate: decisions cite evidence, limitations, owner, and next review date.

## 3. Milestone artifacts

Produce only what helps the next decision:

- Opportunity brief
- Stakeholder, user, scenario, and current-workaround map
- Evidence, assumption, disagreement, and decision register
- Competitor and substitute analysis
- Outcome tree and metric contract
- MVP scope and non-goal list
- Journey, prototype review, requirement list, and acceptance table
- AI decision record, data plan, eval contract, guardrail map, and agent-permission matrix
- Delivery responsibility map and launch-readiness checklist
- Rollout, monitoring, incident, and rollback plan
- Post-launch review and roadmap decision

Keep stage artifacts aligned with the working state. Do not create extra files merely to look complete.

## 4. Ordinary-product adaptation

For a non-AI feature, retain the full product phases and remove AI-only work. Still cover data, permissions, errors, accessibility, analytics, delivery, launch, and iteration. Do not invent an AI layer.
