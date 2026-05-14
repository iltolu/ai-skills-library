# Framework catalog

This catalog explains the core frameworks used by the Ultimate Consultant Skill. Use it as a practical reference, not as a mechanical checklist.

## Core reasoning and communication

### Problem framing and decision framing

**Definition:** Translate a vague issue into a precise decision question with objective, scope, constraints, dependencies, stakeholders, success metric, and time horizon.

**Use when:** The user brings a broad or unclear topic such as “growth strategy,” “operating model,” or “transformation problem.”

**Strengths:** Prevents wasted analysis, creates alignment, and makes trade-offs visible.

**Limitations:** Can feel slow if the user wants an immediate answer. Requires explicit assumptions.

**Implementation steps:**
1. State the decision-maker.
2. Define the decision to be made.
3. List hard constraints.
4. Name the metric and time horizon.
5. Identify what a good answer must decide.

**Prompt pattern:** Rewrite this problem as a decision question with objective, metric, time horizon, constraints, stakeholders, and decision criteria. Flag missing assumptions before analysis.

### MECE

**Definition:** Group ideas so they are mutually exclusive and collectively exhaustive.

**Use when:** Creating categories, workstreams, driver trees, slide headlines, recommendation buckets, or issue trees.

**Strengths:** Reduces overlap, supports parallel work, and improves logical clarity.

**Limitations:** Perfect MECE is often aspirational. Enforcing it too early can suppress creative thinking.

**Implementation steps:**
1. Choose one organizing logic.
2. Test branches for overlap.
3. Test whether a major branch is missing.
4. Relabel branches until the grouping is crisp.

**Prompt pattern:** Organize the answer into MECE buckets. Show where categories overlap, then revise until overlap is minimal and major branches are covered.

### Issue trees and logic trees

**Definition:** A hierarchical decomposition of a problem into branches that can be analyzed separately.

**Use when:** Diagnosing profit decline, churn, market entry, transformation blockers, or operational issues.

**Strengths:** Makes ambiguous problems tractable, creates workstreams, and reveals data needs.

**Limitations:** A bad tree encodes bad assumptions. A neat tree can create false confidence.

**Implementation steps:**
1. Put the core question at the root.
2. Split into top-level branches.
3. Pressure-test MECE.
4. Identify the branches most likely to matter.
5. Convert branches into analyses.

**Prompt pattern:** Build a MECE issue tree for this problem. Label each branch with the evidence needed, likely owner, and expected business impact if true.

### Hypothesis-driven problem solving

**Definition:** Start with candidate explanations or recommendations and test them iteratively instead of collecting data indiscriminately.

**Use when:** Due diligence, diagnostics under time pressure, strategy work, and situations where speed matters.

**Strengths:** Fast, efficient, and action-oriented.

**Limitations:** Can create confirmation bias if alternatives are not actively tested.

**Implementation steps:**
1. State an initial answer.
2. List observable implications.
3. Specify disconfirming evidence.
4. Run the smallest useful test first.
5. Revise hypotheses.
6. Keep a “what changed our mind” log.

**Prompt pattern:** Generate 3 competing hypotheses for the problem, what evidence would support or refute each, and the cheapest next test to discriminate among them.

### 80/20 and Pareto prioritization

**Definition:** Focus on the vital few drivers likely to account for the largest share of the effect.

**Use when:** Prioritizing analysis, narrowing root causes, sequencing a roadmap, or avoiding analysis sprawl.

**Strengths:** Accelerates progress and focuses attention.

**Limitations:** Can miss tail risks, dependencies, or emerging issues.

**Implementation steps:**
1. Estimate impact and controllability.
2. Rank branches by expected value.
3. Select the few high-leverage items.
4. State what is deliberately deferred.

**Prompt pattern:** Rank the branches by likely impact and controllability. Recommend the smallest set of analyses that should explain most of the outcome, and list what we are consciously not analyzing first.

### SCQA and Pyramid Principle

**Definition:** Use Situation, Complication, Question, Answer to frame the audience’s problem, then organize supporting ideas under one clear answer.

**Use when:** Executive memo, synthesis slide, client update, recommendation narrative, or leadership briefing.

**Strengths:** Clear, persuasive, and executive-friendly.

**Limitations:** Can oversimplify if uncertainty and alternatives are hidden.

**Implementation steps:**
1. State the baseline situation.
2. Name the complication.
3. Turn it into the audience’s question.
4. Answer directly.
5. Group supporting arguments under 2–4 top-level messages.

**Prompt pattern:** Respond in SCQA form, then build a pyramid with one answer, three supporting messages, and the evidence needed under each message.

## Analysis and diagnosis

### Decision trees and decision analysis

**Definition:** Map decisions, uncertain events, payoffs, and probabilities to compare alternatives under uncertainty.

**Use when:** Market entry, investment choices, make-or-buy decisions, pilot-or-scale choices, and scenario choices.

**Strengths:** Makes uncertainty explicit and supports expected-value comparison.

**Limitations:** Only as good as inputs. Can become over-precise.

**Implementation steps:**
1. Define alternatives.
2. Specify uncertain events.
3. Assign ranges or probabilities.
4. Estimate payoffs.
5. Compute expected values if appropriate.
6. Run sensitivity analysis.
7. State which assumption most changes the answer.

**Prompt pattern:** Build a decision tree with options, uncertainties, estimated probabilities, expected values, and the two assumptions to stress-test first.

### 5 Whys

**Definition:** Repeatedly ask why to get beyond symptoms to underlying causes.

**Use when:** Process failures, quality issues, operational incidents, service breakdowns, or recurring problems.

**Strengths:** Simple, fast, and accessible.

**Limitations:** Can become too linear, stop too early, or reduce a complex system to one cause.

**Implementation steps:**
1. Define the problem precisely.
2. Ask why iteratively.
3. Verify each answer with evidence.
4. Branch if multiple causes emerge.
5. Stop only at a cause that can be acted on.

**Prompt pattern:** Run a 5 Whys analysis, but allow branching if more than one plausible cause exists. For each why, state evidence confidence and what would falsify it.

### Porter’s Five Forces

**Definition:** Analyze rivalry, threat of entrants, supplier power, buyer power, and substitutes to understand industry structure and profit potential.

**Use when:** Market entry, category attractiveness, pricing power, strategic positioning, and industry economics.

**Strengths:** Strong external-structure lens.

**Limitations:** Weaker for internal capabilities, organization design, and blurred ecosystem boundaries unless paired with other tools.

**Implementation steps:**
1. Define the industry carefully.
2. Assess each force.
3. Identify which forces constrain or protect profit.
4. Note trends changing the forces.
5. Translate into strategic options.

**Prompt pattern:** Apply Five Forces to this industry. Identify the two forces that most constrain profitability, the trend likely to shift them, and implications for market entry or positioning.

### Value chain

**Definition:** Disaggregate a business into strategically relevant activities to find sources of cost advantage or differentiation.

**Use when:** Profit improvement, operating model review, make-or-buy, service redesign, AI automation targeting, or cost transformation.

**Strengths:** Bridges strategy and operations.

**Limitations:** Can understate ecosystems, platforms, or cross-firm effects if used too narrowly.

**Implementation steps:**
1. Map primary and support activities.
2. Estimate cost and value contribution.
3. Locate bottlenecks and differentiators.
4. Translate into redesign actions.

**Prompt pattern:** Map the value chain for this business, identify the three activities most likely to drive cost or differentiation, and recommend what to redesign first.

### 3Cs

**Definition:** Analyze Corporation, Customers, and Competitors as the core strategic triangle.

**Use when:** Growth strategy, positioning, go-to-market simplification, and strategic storyline building.

**Strengths:** Fast, intuitive, and low data burden.

**Limitations:** Lighter than Five Forces for industry economics and lighter than value-chain work for operations.

**Implementation steps:**
1. Summarize company capabilities and constraints.
2. Define high-value customer needs and segments.
3. Compare competitor positions.
4. Identify where all three align to create advantage.

**Prompt pattern:** Analyze this problem through the 3Cs: what matters about the company, customers, and competitors, and where is the most attractive strategic fit?

### 4Ps

**Definition:** Product, Price, Place, and Promotion.

**Use when:** Launch planning, commercialization, demand generation, growth diagnostics, and offer redesign.

**Strengths:** Practical and actionable for marketing choices.

**Limitations:** Product-centric and less useful for broad corporate strategy or internal operating issues.

**Implementation steps:**
1. Define the value proposition.
2. Clarify pricing logic.
3. Define channel and distribution approach.
4. Define promotion strategy.
5. Check consistency across all four levers.

**Prompt pattern:** Use the 4Ps to assess this offer. For each P, identify the current choice, likely weakness, and highest-value change.

### SWOT and TOWS

**Definition:** SWOT inventories strengths, weaknesses, opportunities, and threats. TOWS turns them into strategy options: SO, ST, WO, WT.

**Use when:** Synthesizing after deeper analysis, workshop facilitation, option generation, and planning discussions.

**Strengths:** Broad, accessible, and good for workshops.

**Limitations:** SWOT alone often becomes generic. TOWS is the more useful strategy-generation step.

**Implementation steps:**
1. Build SWOT from evidence already gathered.
2. Generate SO, ST, WO, and WT options.
3. Rank options by feasibility and impact.

**Prompt pattern:** Create a SWOT from the evidence already gathered, then convert it into a TOWS matrix with SO, ST, WO, and WT options ranked by business impact and ease of execution.

## Implementation, governance, and change

### Stakeholder mapping

**Definition:** Identify who matters, what they care about, how much influence they have, and whether they support, oppose, or are neutral.

**Use when:** Transformations, operating-model changes, reorgs, regulator-heavy topics, cross-functional launches, and internal initiatives.

**Strengths:** Reduces political surprises and improves engagement sequencing.

**Limitations:** Stakeholder maps age quickly and can be sensitive.

**Implementation steps:**
1. List stakeholders.
2. Assess power, interest, and stance.
3. Map concerns and incentives.
4. Define tailored engagement actions.

**Prompt pattern:** Create a stakeholder map with role, power, likely stance, key concern, desired action, and next engagement step. Flag likely blockers and coalition builders.

### RACI, RAPID, and decision rights

**Definition:** RACI clarifies Responsible, Accountable, Consulted, and Informed. RAPID-style models clarify decision roles when bottlenecks are the issue.

**Use when:** Implementation governance, transformation offices, operating rhythm, escalation paths, and cross-functional accountability.

**Strengths:** Clarifies accountability and reduces role ambiguity.

**Limitations:** RACI is weaker for contested strategic decisions; decision-rights models need more design effort.

**Implementation steps:**
1. Identify critical decisions or deliverables.
2. Assign ownership.
3. Ensure one accountable owner.
4. Identify required voices.
5. Review bottlenecks after initial use.

**Prompt pattern:** Build a RACI for this initiative. If the challenge is decision bottlenecks rather than task confusion, convert it into a decision-rights map closer to RAPID-style roles.

### OKRs

**Definition:** Objectives are qualitative goals; key results are measurable outcomes.

**Use when:** Strategy deployment, quarterly priorities, transformation tracking, and initiative accountability.

**Strengths:** Aligns teams around outcomes rather than task lists.

**Limitations:** Weak OKRs become KPIs or to-do lists. Bad cascades become bureaucratic.

**Implementation steps:**
1. Define one clear objective.
2. Set 3–5 outcome-based key results.
3. Link team OKRs to enterprise priorities.
4. Review regularly.

**Prompt pattern:** Translate this strategy into OKRs. Write one objective and three to five outcome-based key results, then note what initiatives would most likely move those results.

### McKinsey 7-S

**Definition:** Diagnose organizational effectiveness through shared values, strategy, structure, systems, style, skills, and staff.

**Use when:** Organization design, post-merger integration, operating-model changes, and capability transformation.

**Strengths:** Holistic and useful for diagnosing misalignment.

**Limitations:** Broad rather than sharply causal unless supported by evidence.

**Implementation steps:**
1. Assess each S.
2. Identify inconsistencies.
3. Trace which misalignments most constrain performance.
4. Sequence interventions.

**Prompt pattern:** Run a 7-S diagnosis. Which Ss are aligned, which are not, and which two misalignments most likely explain the performance gap?

### Change models: Kotter, ADKAR, and influence model

**Definition:** Kotter supports mobilization. ADKAR supports individual adoption. Influence-model thinking supports sustained behavior change through conviction, role modeling, formal mechanisms, and skills.

**Use when:** Complex transformations, ERP or AI rollouts, reorgs, cultural shifts, and adoption-heavy initiatives.

**Strengths:** Covers mobilization, adoption, and reinforcement.

**Limitations:** No change model is universal. Local context matters.

**Implementation steps:**
1. Use Kotter to mobilize urgency and coalition.
2. Use ADKAR to diagnose adoption gaps.
3. Use influence-model mechanisms to embed behavior.
4. Define owners and leading indicators.

**Prompt pattern:** Design a change plan using Kotter for mobilization, ADKAR for adoption risks, and an influence-model view for behavior reinforcement. Show actions by phase, owner, and leading indicator.
