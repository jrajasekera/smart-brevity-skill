# Smart Brevity Templates

Use these as working structures, not forms that must be filled mechanically. Replace bracketed prompts, remove empty sections, and adapt labels to the channel. Never invent content to complete a template.

## Executive update

Use for leadership updates, board readouts, operating reviews, and escalations.

```markdown
# [Outcome, variance, risk, or decision]

[State the most consequential result or change in one or two sentences. Include current status and material scope.]

**Why it matters:** [Explain the business, customer, financial, operational, or strategic implication for this leadership audience.]

**By the numbers:**

- **[Most decision-relevant metric]:** [Value, comparison, period, and scope.]
- **[Second metric or threshold]:** [Value and implication.]

**What changed:** [Name the new development, cause only if supported, and any material uncertainty.]

**Decision needed:** [Decision, options if needed, recommendation, decision owner, and deadline.]

**What's next:** [Owner] will [next action or milestone] by [absolute date].

**Go deeper:** [Source of truth, analysis, dashboard, or appendix.]
```

Editorial notes:

- Lead with the outcome or decision, not the team's effort.
- Include only metrics that alter the interpretation or choice.
- State the recommendation when asking executives to decide.
- Surface downside, confidence, and irreversible tradeoffs.

## Project status

Use for recurring updates, milestone checks, delivery changes, and dependency management.

```markdown
# [Project]: [On track / At risk / Off track] for [milestone and date]

[State status versus plan, the most important change since the last update, and the current forecast.]

**Why it matters:** [Explain the effect on users, launch timing, cost, scope, dependent teams, or commitments.]

**Progress:**

- **Completed:** [Outcome completed since the last update.]
- **Next milestone:** [Deliverable, owner, and date.]
- **Key risk:** [Risk, likelihood or evidence, and mitigation.]

**Need from [audience]:** [Specific decision, input, resource, or dependency] by [date].

**Next checkpoint:** [Date/time and what will be known then.]

**Go deeper:** [Plan, tracker, decision log, or technical detail.]
```

Editorial notes:

- Use a status label only when the evidence supports it.
- Report outcomes and forecast changes, not a diary of activity.
- Put the most consequential blocker first.
- Name cross-team dependencies and their owners.

## Decision announcement

Use after a decision is final. For a recommendation awaiting approval, label it clearly as a proposal instead.

```markdown
# [Decision]: [Practical outcome]

[State what was decided, who made the decision if relevant, and when it takes effect.]

**Why it matters:** [Explain the intended result and the consequence for this audience.]

**What changes:**

- **[Area or group]:** [Specific change and effective date.]
- **[Process, product, or policy]:** [Specific change and transition detail.]

**What stays the same:** [Clarify a likely point of confusion, when useful.]

**Action:** [Audience or owner] must [action] by [date]. [Say “No action required” when true and useful.]

**How we decided:** [Decision criteria, strongest tradeoff, and material dissent or uncertainty.]

**Go deeper:** [Decision record, policy, FAQ, or implementation plan.]
```

Editorial notes:

- Do not disguise a proposal as a final decision.
- Explain the rationale without reopening a settled debate.
- Clarify both changes and non-changes when readers may overgeneralize.
- Include transition support for affected people.

## Meeting recap

Use to record decisions, actions, and unresolved issues. Do not reproduce the meeting chronologically.

```markdown
# [Meeting or topic]: [Primary outcome]

[State the most important decision, alignment, or unresolved issue from the meeting.]

**Why it matters:** [Explain what this unlocks, changes, delays, or puts at risk.]

**Decisions:**

- **[Decision]:** [What was decided, scope, and effective timing.]
- **[Decision]:** [What was decided and any condition.]

**Actions:**

- **[Owner] — [Action] — [Deadline].**
- **[Owner] — [Action] — [Deadline].**

**Open questions:**

- **[Question]:** [Owner for resolution and expected answer date.]

**Next checkpoint:** [Date/time, purpose, and required preparation.]

**Go deeper:** [Notes, recording, source document, or decision log.]
```

Editorial notes:

- Separate decisions from discussion.
- Give every action one accountable owner and one date.
- Include only open questions that can change the plan or decision.
- Preserve disagreement when it remains material.

## Incident communication

Choose the internal or customer-facing variant. Use confirmed facts, explicit uncertainty, and a reliable next-update time.

### Internal incident update

```markdown
# [Service or process]: [Current impact and response state]

As of [absolute date and time with time zone], [state the confirmed impact, affected scope, and current response status].

**Why it matters:** [Explain the customer, operational, financial, compliance, or delivery consequence.]

**Current state:**

- **Affected:** [Users, regions, systems, functions, or percentage; include known scope limits.]
- **Mitigation:** [What is being done and whether it is reducing impact.]
- **Known:** [Most important confirmed fact.]
- **Unknown:** [Material uncertainty, including root cause or restoration timing if unconfirmed.]

**Action:** [Specific request to responders, stakeholders, or support teams, with owner and deadline.]

**Next update:** [Date/time and channel], even if the status is unchanged.

**Go deeper:** [Incident record, status page, dashboard, or runbook.]
```

### Customer incident notice

```markdown
# [Product or service] issue affecting [customer-visible function]

Since [time and time zone], some [customers/users] have experienced [plain-language symptom]. We are [investigating / mitigating / monitoring / recovering].

**Why it matters:** [State what customers may be unable to do or what may be delayed.]

**What you may see:** [Observable symptom and known scope.]

**What we're doing:** [Current mitigation or recovery work, without unsupported cause or promises.]

**What you can do:** [Verified workaround or “No action is required.”]

**Next update:** [Date/time and channel].

[Optional, proportionate acknowledgment of disruption and thanks for patience.]
```

Editorial notes:

- Lead with current impact, not internal detection or investigation chronology.
- Never speculate about cause or restoration time.
- Use empathy without diluting the operational facts.
- Keep internal system names, blame, and security-sensitive detail out of customer notices.
- Correct prior statements explicitly when facts change.
