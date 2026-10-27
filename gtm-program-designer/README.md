# GTM Program Designer

> **Status: v0.4, in testing.** Tested blind against two real programs (see "How it was tested"). Feedback very welcome.

Describe a go-to-market priority, such as "lift trial-to-contract conversion across EMEA" or "standardise our prospecting tools", and get a program brief that the field can run, leadership can inspect and finance can believe.

## What it does

1. **Interviews you briefly:** the priority, today's baseline, scope, constraints, other leadership priorities, and how long the sponsor has committed people and budget.
2. **Writes a short brief first** (about two pages): the real problem, objective, business case scenarios, design, governance, time to first result, measurement, top risks and the decisions needed now.
3. **Builds the full brief on request**, in 16 sections, from diagnosis to long-term ownership.

## The thinking behind it

- **Uplift, not activity.** A program is judged by the difference it makes, not the work it ran. So the measurement plan is set *before* launch: baseline, target, a fair comparison (a control group or a staged rollout), a guardrail metric, and how results are attributed.
- **Programs rarely fail on design. They fail on diagnosis, decisions and durability:** solving the wrong problem, leaders not deciding when the field pushes back, and sponsorship ending before results arrive. The skill gives these the same weight as the design itself.
- **Honest numbers.** Every figure is labelled *Given*, *Assumption* or *To confirm*, with the working shown.
- **Built for multi-country regions.** For each component it decides what to run once, what to localise and what to leave to country teams, and it flags where data-protection and consent rules may shape the design.

## The full brief: 16 sections

1. Diagnosis: what is really going on
2. Objective
3. Business case
4. Alignment with other leadership priorities
5. Governance and decision rights
6. Stakeholders, field co-design and alignment
7. Program design: rules (Must, Should, Could), control points, RACI, workstreams, phases
8. Systems and data build
9. Timing: time to first result and the calendar
10. Localisation: run once, localise or leave local
11. Dependencies
12. Barriers, risks and objections
13. Measurement plan
14. Operating cadence
15. Adoption, communication and training
16. Long-term ownership and sponsorship

## How it was tested

The skill was tested **blind** against two multi-market sales programs I led in ad tech:

- I wrote a detailed account of each program from memory, as a story, without looking at the skill.
- A fresh Claude session that had never seen those accounts ran the skill using **only what was known at the start** of each program.
- I compared its brief with what actually happened, listed what it caught, partly caught and missed, and improved the skill.

| Version | Tested against | Fully right | Partly right | Missed |
|---|---|---|---|---|
| v0.1 | A commercial trials program | 3 of 19 | 10 | 6 |
| v0.2 | A sales tooling consolidation program | 10 of 21 | 9 | 2 |

The first test showed that the early version handled *design* well but missed the human side: what the old process was really being used for, governance, markets opting out after launch, calendar freezes, and sponsorship ending before results arrived. The second test showed it now caught most of that, and added recurring yearly processes, capped budgets and measuring the return on each tool. Both programs were different, so the scores aren't a like-for-like comparison, but the direction is clear.

**Checked against public program guidance.** v0.4 was also stress-tested against UK National Audit Office lessons from major programmes, HM Treasury's Green Book (the Five Case Model and optimism bias guidance) and the Magenta Book on evaluation. That added scope and change control, independent checks at key gates, honest status reporting, an explicit allowance for optimistic plans, a theory of change, and a three-question measurement plan.

The blind test also produced things the real programs didn't have, such as a guardrail metric so a program can't "win" by shrinking volume, and default outcomes for undecided escalations.

## Who it's for

GTM programs, sales operations, enablement and revenue leaders who turn leadership priorities into measured programs, especially across many countries.

## Works well with

**Sales Transcript Coach**, in this repository. Together they tell one story: *coach the call → package what works → run it as a measured program.*

## Licence

MIT. Take it, use it, improve it, and please share your feedback.
