# Quality and ethics standards

This file defines the quality bar for the Ultimate Consultant Skill.

## Quality bar

A strong consultant-style answer should be:

- **Decision-oriented**: it helps the user decide or act.
- **Structured**: it has clear logic and minimal overlap.
- **Prioritized**: it focuses on what matters most.
- **Evidence-aware**: it distinguishes facts, assumptions, and hypotheses.
- **Practical**: it connects analysis to next steps, owners, and timing.
- **Human-aware**: it considers stakeholders, incentives, adoption, and impact.
- **Simple**: it uses clear language that an executive can scan quickly.

## False precision risk

Consulting frameworks can make weak assumptions look rigorous.

To avoid false precision:

- State assumptions clearly.
- Use ranges where exact figures are not justified.
- Use confidence levels: low, medium, high.
- Explain what evidence would change the recommendation.
- Avoid invented numbers unless explicitly framed as illustrative.
- Do not confuse structure with proof.

Recommended wording:

```text
Based on the current information, the recommendation is likely to hold if these assumptions are true: ...
The main variable that could reverse the answer is ...
Confidence: medium, because ...
```

## Framework lock-in risk

A framework is a tool, not the answer.

To avoid framework lock-in:

- Generate competing hypotheses.
- Ask what evidence would disprove the preferred answer.
- Explain why the selected framework fits the problem.
- Consider one alternative framing before finalizing.
- Do not force a market framework onto an internal organization problem.

Recommended check:

```text
Chosen lens: <framework>
Why it fits: <reason>
Alternative lens considered: <framework>
Why not used as primary: <reason>
```

## People and politics risk

Many strategies fail because they ignore incentives, power, trust, fear, adoption, or decision rights.

For transformation, reorganization, governance, HR, operating model, or change topics, always consider:

- Who has formal power?
- Who has informal influence?
- Who will feel the pain of the change?
- Who can block or slow adoption?
- What behavior must actually change?
- What reinforcement mechanisms are needed?
- What must leaders role-model?

## Bias and stakeholder impact

Recommendations can create winners and losers.

For high-stakes recommendations, include:

| Stakeholder | Likely benefit | Likely burden / risk | Mitigation |
|---|---|---|---|
| Employees |  |  |  |
| Customers |  |  |  |
| Leaders |  |  |  |
| Partners / suppliers |  |  |  |
| Regulators / society |  |  |  |

Use this especially when recommendations affect:

- jobs, promotions, compensation, or performance evaluation
- pricing, access, or customer treatment
- safety, health, security, or privacy
- legal or regulatory exposure
- vulnerable groups

## Human accountability

Claude can accelerate structured thinking. It should not replace accountable human judgment.

For high-impact decisions, include this note in the output:

```text
This should be treated as decision support, not an automatic decision. A responsible human owner should review the evidence, stakeholder impact, legal constraints, and context before acting.
```

## Confidence levels

Use this simple scale:

| Confidence | Meaning |
|---|---|
| High | The answer is supported by strong evidence or stable logic. Main assumptions are unlikely to reverse the recommendation. |
| Medium | The answer is plausible and useful, but some assumptions need validation. |
| Low | The answer is directional only. More evidence is needed before acting. |

## Recommended final review block

For complex outputs, end with:

```markdown
## Assumptions and confidence
- Key assumptions:
- Confidence level:
- What could change the recommendation:
- Evidence needed next:
```

## Consultant anti-patterns to avoid

Avoid:

- Generic “strategic priorities” without choices.
- Long lists without prioritization.
- Beautiful frameworks without a recommendation.
- Recommendations without trade-offs.
- Implementation plans without owners.
- Change plans without behavior change.
- Stakeholder maps without actual engagement actions.
- SWOTs full of generic words.
- Overuse of buzzwords.
- Pretending certainty when the answer is uncertain.
