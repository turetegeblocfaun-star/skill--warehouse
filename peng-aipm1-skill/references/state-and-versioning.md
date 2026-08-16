# Working State, Traceability, and Versioning

## Contents

1. Working-state schema
2. Traceability rules
3. Working-version rules
4. Mandatory turn footer
5. Recap and milestone format

## 1. Working-state schema

Maintain this logical state throughout the conversation. Do not dump it on every turn.

- Product or feature name
- One-sentence product logic
- Current lifecycle phase and gate
- Confirmed facts and external evidence
- User judgments and preferences
- AI hypotheses and recommendations
- Assumptions and validation status
- Stakeholders, users, scenarios, needs, and current workarounds
- User, business, quality, safety, system, and cost outcomes
- Candidate ideas, current scope, later scope, non-goals, and rejected alternatives
- Decisions with owner, rationale, evidence, date, and version
- Disagreements and evidence that would resolve them
- Requirements, acceptance conditions, dependencies, risks, and owners
- AI design, data, eval, safety, agent, cost, and rollout state when relevant
- Parking lot
- Stage artifacts produced
- AI product manager growth evidence
- Working version and change history

When context is incomplete, reconstruct from the visible conversation and mark uncertainty. Do not silently overwrite an earlier decision.

## 2. Traceability rules

Every material final statement must trace to at least one of:

- A user-provided fact
- A user-owned decision
- A cited external source
- A clearly labeled AI recommendation
- A clearly labeled assumption with a validation plan

When a decision changes, preserve the old view, new view, reason, and consequence. Show this evolution in the learning document; show only the current decision and relevant history in the professional document.

Keep professional, learning, stage, and recap artifacts aligned. A version update is incomplete if one artifact still carries a superseded user, scope, metric, architecture, or risk decision.

## 3. Working-version rules

Use semantic working versions for the evolving AI Feature PRD. Start at `v1.0.0` when the first substantive project state is created.

- **Patch:** Small clarification, added example, refined wording, or detail within an existing module. Example: `v1.1.0 → v1.1.1`.
- **Minor:** New capability, lifecycle module, material decision, scope change, architecture choice, evaluation plan, or substantial batch of content. Example: `v1.1.1 → v1.2.0`.
- **Major:** Fundamental change to target user, core problem, product positioning, or document architecture that invalidates major prior work. Example: `v1.x.x → v2.0.0`.
- **No change:** Discussion, question, or explanation that adds no accepted fact, decision, assumption, evidence, candidate, or requirement. Keep the version and say so.

Do not increment merely because a turn occurred. Choose the version after evaluating the actual change size.

The working-document version is not the Skill's installed release version. Never imply that the Skill itself has been updated during product coaching.

## 4. Mandatory turn footer

End every user-facing turn with one of these natural-language notices.

For a changed working state:

```markdown
> 已把 AI Feature PRD 工作稿更新到 vX.Y.Z  
> 本轮更新：{{具体新增、修改或推翻的内容}}
```

For no substantive change:

```markdown
> AI Feature PRD 工作稿仍为 vX.Y.Z  
> 本轮未形成新的产品共识，版本未变化。
```

Before the project state exists:

```markdown
> AI Feature PRD 工作稿尚未建立版本  
> 当前进展：正在确认第一个产品事实或方向。
```

Keep the footer concise and accurate. Do not expose internal Skill storage, repository, or implementation details.

## 5. Recap and milestone format

Use this structure when the user requests progress or a phase gate is reached:

```markdown
当前阶段
- ...

已确认
- ...

外部证据
- ...

待验证假设
- ...

仍有分歧
- ...

已做决定
- ...

候选与停车场
- ...

当前最大风险
- ...

下一项关键决定
- ...
```

Include only non-empty groups. Finish with the version footer.
