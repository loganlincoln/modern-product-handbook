# Product Lifecycle & Practices

This section outlines an end-to-end, organisation-agnostic playbook for building products with clarity and consistency. The lifecycle is not a strict sequence; it is a continuous loop that starts with a customer problem and continues through delivery, launch, and iteration.

A useful shorthand: **problem → evidence → decision → delivery → impact → learning → (back to problem)**.

## Lifecycle stages (problem to impact)

| Stage | Focus | Typical activities |
|---|---|---|
| Discovery | Understand the problem | Problem framing, interviews, journey mapping, prototyping, assumption testing, competitive research. |
| Business viability | Confirm the business case | Market sizing, unit economics, pricing/packaging hypotheses, buy/build/partner options, risk & compliance checks. |
| Planning & prioritisation | Decide what to do next | Outcome setting, roadmap creation, OKRs, trade-off analysis, sequencing, dependency management. |
| Execution & delivery | Build the solution | Backlog refinement, sprint/kanban execution, quality practices, risk management, cross-functional alignment. |
| GTM strategy & enablement | Prepare to launch | Positioning/messaging, enablement materials, launch planning, internal training, customer comms planning. |
| Launch & optimisation | Ship and learn | Release readiness, rollout strategy, monitoring, adoption analysis, post-launch reviews, iterative improvement. |

---

## 2.1 Product backlog vs delivery backlog

Many teams rely on a single, catch-all backlog where ideas, bugs, strategy, and delivery tasks compete in the same list. That often leads to confusion, inconsistent priorities, and decisions driven by urgency or the loudest voice.

A practical alternative is to maintain two related (but distinct) backlogs:
- **Product backlog**: strategic thinking and evidence (the “what and why”).
- **Delivery backlog**: build commitments and execution work (the “how and when”).

### Product backlog (the “what” and “why”)

The product backlog is a long-lived space for shaping opportunities. It is typically owned by the product manager (or product trio) and exists to answer:

> What should be invested in, and why?

**What it contains**
- Ideas: early signals, one-liners, raw feedback.
- Problems/opportunities: clearer statements of unmet needs and target users.
- Solution hypotheses: candidate approaches to test.
- Evidence: research notes, analytics insights, customer quotes, experiment results.
- Decision context: trade-offs, constraints, risks, assumptions.

**How to organise it (two simple options)**
- **By size**: Boulders (large bets), Rocks (mid-sized), Pebbles (small fixes).
- **By maturity**: Long list (someday/maybe), Medium list (promising), Short list (next to validate or deliver).

### Delivery backlog (the “how” and “when”)

The delivery backlog is a short-term commitment tool for building and shipping. It is often owned by engineering (or the delivery lead) and exists to answer:

> How and when will the team deliver?

**What it contains**
- Epics, stories, tasks, sub-tasks.
- Bugs and operational work.
- Technical enablers (refactors, platform work, reliability work).
- Release and rollout tasks.

**How it is used**
- Execute and track day-to-day progress.
- Sequence work based on dependencies and capacity.
- Coordinate delivery milestones and releases.

A healthy system keeps the two backlogs linked: delivery work should trace back to an objective, problem, or hypothesis in the product backlog.

---

## 2.2 Discovery

Discovery is the continuous practice of understanding customers and reducing risk before (and while) building. It is not a one-time phase; it runs in parallel with delivery so teams can keep learning, validating, and refining direction.

Discovery is the antidote to expensive mistakes: it is usually cheaper to learn through a prototype or experiment than through fully shipped software.

### Discovery principles

- **Minimise waste**: validate to build, not build to validate.
- **De-risk early**: identify the biggest risks first and seek evidence quickly.
- **Prefer evidence over debate**: resolve uncertainty through learning.

### Key risk categories

Most product work carries four classic risks:
- **Value risk**: Will customers choose it or pay for it?
- **Usability risk**: Can customers understand and use it successfully?
- **Feasibility risk**: Can the team build and operate it?
- **Viability risk**: Will it work for the business (legal, security, commercial, brand, support)?

For AI-enabled products, add three common AI-native risks:
- **Reliability risk**: outputs can be probabilistic and inconsistent; the system can be confidently wrong.
- **Bias/safety risk**: outputs can reflect bias or produce harmful content.
- **Adversarial risk**: the system can be manipulated (e.g., prompt injection) or leak sensitive data.

### An idea lifecycle (a shared vocabulary)

A lightweight way to track “where an idea is” is to use four stages. Teams can move back and forth between them as they learn.

1. **Frame** (Is it worth solving?)  
   Clarify the user, the problem, and why it matters now. Define what evidence would justify investment.

2. **Explore** (Is this the right solution?)  
   Test assumptions with prototypes and experiments; narrow to approaches that can work.

3. **Make** (Are we building it right?)  
   Build and iterate with strong collaboration, quality practices, and clear success measures.

4. **Impact** (Is it delivering value?)  
   Measure adoption and outcomes; iterate, pivot, or stop based on evidence.

### Practical discovery techniques

Use the smallest credible technique that answers the biggest question:
- Customer interviews and workflow observation.
- Prototype tests (low to high fidelity).
- Concierge / manual workflows to validate demand.
- Wizard-of-Oz tests to validate the experience before automation.
- Limited rollouts and controlled experiments.

### Collaboration rituals that help discovery

Discovery is a team sport. The fastest teams build shared context early and avoid handoffs.

Helpful habits:
- Include engineering and design in early customer learning when possible.
- Separate **divergent exploration** (generate options) from **convergent alignment** (choose and commit).
- Use lightweight, written decision records so context survives team changes.

---

## 2.4 Continuous feedback & insights

Continuous feedback is the engine that keeps the product lifecycle honest. It ensures decisions stay grounded in customer reality and measurable evidence—rather than opinions, anecdotes, or organisational noise.

A healthy insight loop improves prioritisation, builds trust through shared context, and reduces the risk of over-indexing on any single source (e.g., one enterprise customer, one loud stakeholder, or one dashboard).

### Establish continuous feedback channels

Create dedicated channels that capture different “shapes” of feedback—qualitative and quantitative, inbound and outbound, reactive and proactive. The goal is not to collect everything; it’s to reliably collect enough signal to make better decisions.

Recommended channels:
- **Inbound user feedback**
  - In-product feedback widgets, a feedback portal, support tickets, community posts.
- **Internal (frontline) feedback**
  - Structured intake from sales, support, and customer success (form + triage rhythm).
- **Surveys**
  - Target cohorts based on segment and behaviour; recurring pulses and one-offs.

Suggested operating habits:
- Tag feedback consistently (theme, segment, severity).
- Separate feedback collection from roadmap commitment.
- Close the loop when possible: “heard → considered → shipped (or not) → why”.

### Collaborate with lighthouse users

Lighthouse users are a small set of customers who act as high-signal partners—especially during discovery, early delivery, and iteration.

How to select lighthouse users:
- Clear communicators who can articulate pain and workflow context.
- In the target segment (or the segment being expanded into).
- Strongly affected by the problem being solved.
- Comfortable with early-stage experiences and some rough edges.

How to work with lighthouse users:
- Set up a dedicated communication path and regular check-ins.
- Share early concepts and prototypes before building.
- Offer early access via alpha/beta programs with explicit expectations.
- Close the loop: show what changed because of their input and what didn’t (and why).

---

## 2.5 Planning & prioritisation

Planning and prioritisation turns insights and validated problems into a clear, actionable plan. It is the discipline of choosing where to invest (and where not to), based on strategy, evidence, constraints, and measurable outcomes.

This practice is built on three pillars:
1. Strategic roadmapping
2. Prioritisation frameworks
3. Goal setting (OKRs or equivalent)

### Strategic roadmapping

A product roadmap is a strategy communication tool. It should explain where the product is going and why, connect work to outcomes, and provide enough clarity for teams and stakeholders to align—without pretending the future is fully knowable.

Core components:
- **Vision**: a clear narrative of the future you are trying to create and for whom.
- **Outcomes**: measurable results (activation, retention, task success, revenue, cost-to-serve, reliability).
- **Time horizons**:
  - **Now**: committed work currently in delivery.
  - **Next**: validated opportunities with flexibility in scope/sequence.
  - **Later**: themes and bigger bets with higher uncertainty.

A useful connecting structure (optional): **Outcome → Opportunities → Solutions → Experiments**.

Roadmapping practices that tend to work:
- Start with the “why” (vision and outcomes), then derive initiatives.
- Frame items as problems to solve, not fixed feature lists.
- Build with cross-functional partners to surface constraints early.
- Communicate frequently using the simplest view each audience needs.

### Prioritisation frameworks

Prioritisation is choosing intentionally under constraints. The goal is not perfect scoring; it’s defensible decisions and clear trade-offs.

Common frameworks (pick what fits; avoid running all of them at once):
- **RICE**: (Reach × Impact × Confidence) / Effort
- **Kano**: Basic needs / Performance / Delighters
- **ICE**: Impact / Confidence / Ease
- **RUF**: Reliability / Usability / Features
- **The $10 game**: budget allocation + reasoning discussion

Practical prioritisation guardrails:
- Make trade-offs explicit (what is not being done, and why).
- Treat estimates as hypotheses; revisit when evidence changes.
- Separate severity (pain) from value (impact) and effort (cost).

### Goal setting (OKRs or equivalent)

Goals translate strategy into measurable intent. OKRs are one common format.

A pragmatic approach:
- **Objectives**: qualitative, time-bound, outcome-oriented.
- **Key results**: 2–3 measurable indicators per objective.
- **Alignment**: connect team goals to portfolio/company strategy.
- **Cadence**: review regularly and reflect at cycle end.
- **Grading**: use a consistent method to assess progress and learn.

---

## 2.6 Execution & delivery

Execution is where strategy becomes tangible. It is the discipline of turning validated problems and hypotheses into high-quality, customer-facing outcomes—reliably and repeatably.

Discovery helps teams build the right thing; execution helps teams build the thing right.

### Core delivery principles

- **Small, frequent, uncoupled releases**  
  Deliver in increments that reduce risk, enable fast feedback, and keep change sets easy to understand and roll back.

- **Instrumentation**  
  Build measurement in from the start so teams can understand behaviour, validate hypotheses, and quantify impact.

- **Monitoring**  
  Detect issues early with observability and alerting. Monitor not just “did it ship?” but also reliability, performance, and (when relevant) model quality and cost.

### Delivery practices

#### Backlog management

Backlog management keeps delivery clear and predictable.

Practices:
- Write clear, actionable stories (who/what/why).
- Make all work visible (reliability, platform, enablement, AI iteration work where relevant).
- Use a Definition of Ready (DoR).
- Refine continuously with engineering and design.

**Definition of Ready (standard)**
A delivery item is typically “Ready” when:
- The user and problem are clear.
- Acceptance criteria are testable.
- Dependencies and risks are identified (and have owners).
- Designs/content are sufficient (or explicitly deferred).
- Instrumentation/measurement needs are defined.
- The team agrees it can be delivered within the intended slice.

**Additive DoR for AI-enabled features (recommended)**
Consider adding:
- Data and privacy approach documented.
- Evaluation approach defined.
- Quality target stated.
- Baseline prompts/configs captured.
- Failure-mode UX designed.
- Safety/misuse risks reviewed.
- Cost and latency expectations defined.

#### Operating rhythm (sprints, flow, and releases)

A delivery cadence is the team’s heartbeat: plan, execute, review, and improve.

Common elements:
- Planning (capacity, priorities, dependencies).
- Daily coordination (surface blockers early).
- Review/demos (what shipped and what changed).
- Retrospectives (improve the system).

For AI-enabled teams, add a deliberate “quality loop”:
- Review quality against the evaluation approach.
- Track failure modes and trends.
- Monitor cost/latency and adjust as needed.

Release habits that support speed and safety:
- Prefer incremental releases over big-bang launches.
- Use feature flags, staged rollouts, and rollback plans where appropriate.
- Treat release readiness as a checklist (quality, monitoring, comms, support readiness).

#### Cross-functional alignment

Execution is a team sport. Product leaders act as integrators.

Alignment techniques:
- Proactive dependency management.
- Single source of truth (objectives, decisions, status, release notes).
- Lead with a shared narrative (problem, outcome, trade-offs).
- Clarify responsibilities when complexity rises (e.g., RACI).

---

## 2.7 GTM strategy & enablement

In many organisations, GTM is treated as downstream: product builds, then marketing and sales “launch it.” That handoff model is a common cause of weak adoption, confused messaging, and missed revenue.

A stronger approach is to treat GTM, marketing, sales, and customer success as partners in the outcome from day zero.

This approach is built on:
- **Early co-ownership** (alignment before build, not after)
- **Artifact-driven clarity** (shared documents that create a single source of truth)

### Artifact-driven alignment (narratives + FAQs)

A high-leverage pair:
- **Launch narrative** (press-release style)
- **FAQ** (hard questions answered in advance)

Suggested FAQ prompts:
- Who is the customer?
- What do they do today?
- Why adopt now?
- How will it be packaged/priced?
- What does success look like?
- What are key risks?
- What will sales/support need?

### Positioning and messaging

Useful components:
- Positioning statement (internal anchor: audience, problem, promise, differentiation)
- Core value proposition (external message, consistent across channels)
- Buyer journey (awareness → evaluation → purchase → onboarding → value realised)

### Sales and channel enablement

Common enablement assets:
- Sales playbook (personas, qualification, objections)
- “Why buy” story/deck (outcome-led narrative)
- Demo narrative (workflow and value, not feature tours)
- Implementation/support guidance (time-to-value, pitfalls, escalation)

Enablement rituals:
- Training sessions (Q&A and role-play)
- Single source of truth for assets
- Field feedback loop (objections, confusion, lost deals)

### Ongoing growth and retention

Sustained growth requires:
- Clear growth metrics (activation, engagement, retention, expansion, churn, revenue)
- Retention and onboarding improvements (reduce time-to-value)
- An optimisation roadmap (adoption blockers and friction as growth work)
- Continuous feedback loops

---

## 2.8 Launch & optimisation

Launch is the moment a product meets real users at scale—and where the real lifecycle begins. It is more than “shipping code”: it is the coordinated rollout of value, the measurement of impact, and the iteration that turns a release into sustained outcomes.

This stage applies to everything from a small improvement to a major new product.

### Pillar 1: release & communication plan

A release plan aligns cross-functional partners on:
- Audience and messaging
- Rollout strategy (staged rollout, safety mechanisms, rollback plan)
- Cross-functional activities and owners
- Success metrics (leading and lagging indicators)

Practical guidelines:
- Collaborate early.
- Keep it concise.
- Define “release” holistically (readiness + learning plan).

### Pillar 2: performance monitoring & feedback loops

Monitoring should answer:
- Is it working reliably?
- Are customers adopting it?
- Is it delivering outcomes?
- What is breaking or confusing?

Core activities:
- Define key metrics before launch.
- Build an analytics view (dashboard or recurring report).
- Maintain continuous feedback channels.
- Run controlled optimisation where appropriate.

**Additive monitoring for AI-enabled products (recommended)**
Include:
- Quality signals (evaluation pass rates, failure modes)
- Safety signals (misuse, policy violations, harmful outputs)
- Cost signals (cost per interaction, latency distributions)
- Drift signals (changes in input patterns and output behaviour)

### Pillar 3: post-launch reviews

A post-launch review is for learning and accountability, not blame.

Suggested agenda:
1. Revisit the original hypothesis
2. Review the data
3. Synthesize learnings
4. Decide next steps (iterate, expand, pivot, stop)

Outputs:
- A short written note with metrics, decisions, and follow-ups
- Updated assumptions and roadmap priorities

### Optimisation for AI-enabled products (defensive + proactive)

AI-enabled experiences can degrade due to drift. Optimisation includes:
- Defensive maintenance (preserving baseline quality)
- Proactive improvement (better UX, trust, cost efficiency)

Two continuous loops help:
- **Model quality loop**: monitor → detect drift → act
- **Human-in-the-loop loop**: route → review → feedback (to improve prompts, UX, policies, and where applicable training data)
