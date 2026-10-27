# Sales Transcript Coach

Paste in a sales call transcript and get coached the way a great sales manager would coach you: on *how you handled the call*, stage by stage, with the evidence behind every score and specific things to try next time.

## What it does

1. **Choose a coaching methodology.** The built-in one describes how a well-run call flows across seven stages: opening and agenda, discovery, listening and confirming, tailored value, handling objections, commercial discipline, and close and next step. What "Strong" looks like at each stage changes with the call type (Discovery, Demo/Technical, Proposal/Pricing or Negotiation/Close), so a closing call is never judged by discovery standards. Or describe your own call playbook, and Sales Transcript Coach turns it into a scoring rubric and checks it with you first.
2. **Add a transcript.** It's the only required input. Add the call type, or a CRM record, for a sharper review.
3. **Get the review.** Each stage is scored 2 (Strong), 1 (Partial) or 0 (Missing), with the moment from the call that earned it. You get a call quality score with the working shown, and two or three coaching points written as *Situation – Behaviour – Impact – Try this*, each with an example line to use next time. A secondary MEDDIC check shows what the call achieved for the deal, alongside flags for commercial errors and risks, next actions and a short briefing written to the rep.

## Why it's built this way

- **Coach the behaviour, not just the deal.** Sales methodologies like MEDDIC tell you what a deal is missing. A coaching methodology tells you *why*: what the rep did or didn't do on the call. Sales Transcript Coach leads with the behaviour and uses MEDDIC as the second lens.
- **A fixed rubric, not opinions.** Without a written framework, an AI will score the same call differently each time. Writing the rules into the skill makes scores consistent and comparable across calls and reps.
- **Evidence for every score.** A rep can argue with a number, but it's much harder to argue with their own words. Quoting the moment builds trust in the coaching.
- **Simple, checkable maths.** Points out of points available, shown in full, so anyone can verify a score by hand.
- **Commercial errors come first.** An unauthorised discount or promise can cost more than any missed question, so it's flagged before anything else.

## How it was tested and refined

- **Blind-tested on court transcripts:** run on anonymised Supreme Court oral arguments (public domain, with known outcomes) using a custom "persuasion under questioning" methodology. The scores didn't predict the outcomes, because courts decide on the law rather than performance, which confirmed an important principle: the coach measures the rep's craft, not the deal's fate. The test also exposed gaps that are now fixed: scoring stages that happen many times in one call, transcripts that stop early, buying committees and non-sales contexts.
- **Checked against the Calgary-Cambridge guide,** the research-based framework used to train doctors in structured consultations. It shares a similar shape and added: getting all concerns on the table at the start, exploring the buyer's ideas, concerns and expectations, picking up cues, explaining in small checked chunks, planning for things going wrong at the close, and the two threads of structure and relationship that run through every call.

## How it was built

Sales Transcript Coach grew out of the *AdCorn AI Deal Coach*, a portfolio build in which a fictional ad tech company, three CRM opportunities and six realistic call transcripts were used to design and test an AI coaching system. Across three deals at different health levels (stalled, qualify-out risk and progressing), the coach had to tell them apart, not just describe them. In testing, it independently spotted a rep implying a minimum fee was negotiable without sign-off, which is why commercial-error detection is built in.

This public version keeps that coaching approach, removes the company-specific details, needs only a transcript to run, and lets you bring your own framework.

## How to start it

Claude picks the skill up automatically when you share a sales call transcript, or when you say things like:

- "Coach me on this call" · "Coach my rep on this transcript"
- "Review / score / grade / rate this sales call"
- "How did my call go?" · "What could I have done better?"
- "Give me feedback on my discovery call / demo / pricing call / negotiation / closing call"
- "Call review" · "Call scorecard" · "Call coaching" · "Sales coaching" · "Deal coaching"
- "Run a MEDDIC check on this call" · "Did I qualify this deal?"
- Or by name: "Use Sales Transcript Coach"

## Getting the best results

- **Speaker labels with names are essential.** Sales Transcript Coach needs to know who the rep is and who said what. A transcript without speaker labels can't be coached fairly, so it will ask you first.
- **Any format is fine:** pasted text, a Word or PDF file, or exports from Gong, Zoom, Teams, Fathom and similar tools.
- **A short header helps:** list the attendees, their roles and the call type (Discovery, Demo/Technical, Proposal/Pricing or Negotiation/Close).
- **Timestamps are helpful but optional.**

## Try it with the examples

The `examples` folder holds two fictional call transcripts, each paired with the review Sales Transcript Coach produced:

| Transcript | Review | What it shows |
|---|---|---|
| `bloom-wellness-call2-transcript.md` | `bloom-wellness-call2-review.md` | A pricing call that slipped: 57% (Developing), with a commercial error caught |
| `crestline-digital-call2-transcript.md` | `crestline-digital-call2-review.md` | A tough call handled well: 79% (Strong) |

Paste either transcript into Claude with the skill installed and compare your result with the saved review. Together they show the skill telling a weak call from a strong one.

## Who it's for

Sales Transcript Coach is built for **GTM programs, sales enablement and sales leadership teams** who want every call coached to the same standard, at scale. It turns a house call methodology into a consistent, evidence-based review that a manager would otherwise spend an hour writing. It's equally useful for an individual seller who wants honest feedback after every call.

## What it draws on

Only what you give it: the transcript, an optional CRM record and an optional custom framework. Nothing is stored unless you save it yourself.

## Ideas for using it

- Self-coaching after every discovery call
- Weekly call reviews in team one-to-ones
- Onboarding new sellers against your house methodology
- Adapting the same pattern to customer success, recruitment or negotiation calls, by swapping in a different framework

## Licence

MIT. Take it, use it, improve it, and please share your feedback.
