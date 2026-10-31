# Career 180 Case Study: "The Completion Trust Problem"

## Who They're Looking For

- 3–4 years of product management experience
- Strong product discovery skills: able to identify the real problem before jumping to solutions
- Able to make clear product decisions, balance stakeholder priorities, and explain trade-offs
- Experience with EdTech, SaaS, LMS, MOOCs, career development, or skills-based platforms is a plus
- Comfortable using AI tools to prototype ideas, explore solutions, and turn concepts into tangible product experiences
- Data-driven mindset: able to conduct research, analyze product metrics, validate assumptions, and iterate based on evidence
- Strong communication skills, able to explain complex ideas clearly and concisely

---

## The Challenge: "The Completion Trust Problem"

### The Story

Learners finish courses and get certificates, but completed is not the same as competent. Completion based on watching videos is easy to game: skip ahead, leave a tab open, click through a quiz. As the platform grows and works with employers, corporate training buyers, and hiring channels, this becomes a trust problem. A partner asks, reasonably:

> "If someone shows us a certificate, does that actually mean anything?"

Three internal stakeholders care about the answer, and they want different things:

| Stakeholder | Wants | Why |
|---|---|---|
| Content & Instructors | Completion stays low-friction | Instructor payouts and rankings are tied to completion rate; mandatory assessments would tank it |
| Employer Partnerships | Certificates that are concrete and defensible | A corporate buyer has already asked how completions are verified |
| Growth & Marketing | The "certified learners" number keeps climbing | It's a headline metric in every pitch; a stricter bar shrinks it |

Nobody is being unreasonable. Somebody still has to decide what a certificate should actually mean. **You're that somebody.**

### What You Need to Solve

Design and prototype a way for a partner (employer or hiring channel) to check a certificate and understand how much to trust it, such that:

- The trust signal is based on evidence, not just a completed-course flag.
- It works across a catalog with uneven assessment depth: some courses have no assessment, some have an auto-graded quiz, a few have a proctored or project-based exam. You can't redesign every course.
- It has a position on certificates already issued under the old, looser standard.
- It's an MVP that a small team (about 2 backend + 1 frontend engineer) could ship in one quarter.

### Real-World Conditions

- Thousands of courses of varying age and quality
- Roughly a third of learners come through corporate accounts where an employer enrolls staff in bulk; their engagement is lower and harder to separate from genuine effort
- Instructor contracts often tie payout to completion rate, so you can't unilaterally redefine "complete" everywhere
- Certificates have no expiry or versioning today; if a course is revised later, old certificates have no defined relationship to the new standard
- Legal requires a defensible methodology behind any "verified" claim

The brief gives no exact numbers. Where your design depends on one, **state your assumption and say how you'd check it.**

### Rules Left Unspecified (On Purpose)

We're not telling you:

- What separates a trustworthy completion from an ordinary one, or whether to use tiers at all
- How to treat courses with no assessment
- What happens to old certificates: grandfather, re-evaluate, downgrade, or something else
- How to weigh instructor incentives against partner trust
- Whether corporate learners are treated differently
- Where the MVP cutline sits

Make a reasonable decision, document it, and move forward. Please don't contact them for clarification. How you handle ambiguity is part of what's being evaluated. (Questions about logistics or format are welcome until the registration deadline.)

---

## What to Hand In

### D1. Decision Memo
**Limit:** Maximum 4 pages

Must include:

- Your trust model and how it handles courses with no assessment.
- Your position on certificates already issued.
- Your decision on the conflict between Content, Partnerships, and Growth, including who bears the cost and roughly how much.
- Your MVP scope for one quarter, with 2 backend engineers and 1 frontend engineer.
- Each key claim labeled as either backed by the brief or an assumption.

### D2. MVP PRD
**Limit:** Maximum 5 pages

Must be written so engineering can start without a meeting. Include:

- Certificate states and transition rules.
- Required data changes.
- Migration of existing certificates.
- Acceptance criteria for each MVP item.

### D3. Discovery and Validation Plan
**Limit:** Maximum 2 pages

Include:

- Your three riskiest assumptions.
- Who you would talk to.
- What results would make you change your design.

### D4. Working Prototype
**Limit:** A link or a screen recording of 3 minutes or less

Build a certificate verification experience that allows a partner to:

- Enter a certificate ID.
- See the verification outcome and the evidence behind it.

Requirements:

- Use 20–30 sample records you create.
- Cover courses with no assessment, auto-graded quizzes, and proctored or project-based exams.
- Include corporate and self-directed learners.
- Include a course revised after certificates were issued.
- Submit the sample data with the prototype.

Any tool is acceptable; production code is not required.

### D5. Three Diagrams
**Limit:** 1 page each

- **Trust Model:** Inputs, rules, and certificate outcomes for each path.
- **Certificate Lifecycle:** Each state and the event that moves a certificate between states.
- **Partner Verification Flow:** Every step from receiving a certificate to accepting or disputing it.

### D6. Metrics Table
**Limit:** Maximum 1 page

Include:

- One north star metric.
- 2–4 guardrail metrics.
- At least one metric that reveals whether trustworthy completions are failing in practice.
- The threshold that would trigger a change to the model.

### D7. Edge Case and Policy Register
**Limit:** 5–8 rows

For each case, describe the scenario and your proposed handling.

Must include:

- A course with no assessment.
- A course revised after certificates were issued.
- At least 3 additional edge cases of your own.

### D8. AI Usage Note
**Limit:** Maximum half a page

Explain:

- Where AI helped you.
- One AI suggestion you rejected and why.

### D9. Unasked Question
**Limit:** Maximum half a page

Identify one risk, question, or opportunity not raised in the brief, explain why it matters, and describe the first action you would take.

### D10. Working Log
**Limit:** Maximum 1 page

Document each work session, including:

- Date.
- Start and end times.
- What you worked on.
- What you cut and why.

### Senior Bonus (Optional, Not Scored)

Six months after launch, a major corporate partner says several people they promoted based on "trusted" certificates underperformed, and they're threatening to pause the partnership. Be ready to discuss:

- How you'd tell whether this is a flaw in the trust model, a data problem, or a mismatch in partner expectations.
- What you'd change.

---

## AI Usage Policy

AI tools are fully allowed and encouraged: for research, drafting, and especially for building your prototype. They're not evaluating whether you used AI. They're evaluating whether the **judgment is yours**. In the live review, expect to explain why you made your key decisions and where you overrode AI.

## Tech Stack

None required. This is a product role, so use whatever lets you build and test fastest (AI app builders, Figma, no-code tools, spreadsheets, or simple code). You should be comfortable with a typical LMS/EdTech setup: course catalog, assessments, certificate issuance, corporate accounts, basic analytics.

---

## What You Should Submit

**One link** (anyone-with-link view, English) containing:

- Problem & Solution Brief
- Link to the working prototype, plus the sample data
- Validation & Iteration Note
- Demo video link

You keep the rights to your work, and Career-180 won't use it commercially.

---

## Evaluation Criteria

| # | Criterion | Weight |
|---|---|---|
| 1 | Strategy and Decision Quality | 25% |
| 2 | Prioritization and MVP Scoping | 20% |
| 3 | Discovery and Assumption Handling | 15% |
| 4 | Metrics and Analytics | 15% |
| 5 | Requirements Clarity (PRD, Diagrams, Prototype) | 15% |
| 6 | Edge Cases and Risk | 10% |

---

## Deliverables Checklist

- [ ] D1. Decision Memo (≤ 4 pages)
- [ ] D2. MVP PRD (≤ 5 pages)
- [ ] D3. Discovery and Validation Plan (≤ 2 pages)
- [ ] D4. Working Prototype (link or ≤ 3 min recording) + sample data (20–30 records)
- [ ] D5. Three Diagrams (Trust Model, Certificate Lifecycle, Partner Verification Flow; 1 page each)
- [ ] D6. Metrics Table (≤ 1 page)
- [ ] D7. Edge Case and Policy Register (5–8 rows)
- [ ] D8. AI Usage Note (≤ ½ page)
- [ ] D9. Unasked Question (≤ ½ page)
- [ ] D10. Working Log (≤ 1 page)
- [ ] Final submission: single anyone-with-link doc (English) with brief, prototype + data links, validation note, demo video
