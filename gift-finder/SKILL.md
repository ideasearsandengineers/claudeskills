---
name: gift-finder
description: Find a thoughtful, creative gift for a specific person and occasion (birthday, Christmas, anniversary), keeping a private record of people, past gifts and rejected ideas so every run gets smarter. Use when the user asks for gift or present ideas.
---

# Gift Finder (v1.1)

Purpose: help the user give a gift that answers a small, meaningful detail the recipient thought nobody noticed, in about 5 minutes for a new person and 2 minutes for a repeat. The best idea often comes from the user; the skill's job is to spark it.

Created by Greg Cristal. Shared under the MIT Licence.

## What you need
- **Recommended:** a Google Drive / Google Sheets connection, so the skill can keep a private memory of people, gifts and rejections between runs.
- **Without it:** the skill still works. Keep the record in the conversation and, at the end, give the user paste-ready rows to save wherever they like.
- **Web search**, for finding real products and bookings in Step 5.

## Question style (applies to every screen)
- Ask up to 4 multiple-choice questions per screen, using the app's question tool where available (otherwise as a short numbered list). The user can always give their own answer.
- Every option is a vivid, concrete scene, never an abstract trait. Ask "When did you last see them genuinely light up?" not "Practical or sentimental?"
- Only one short typed answer per run, in detail-mining (Step 4).

## Step 0 - Find or create the private record
1. If Google Drive is connected, search for a sheet named "Gift Finder". If found, connect to it. If not, create it with four tabs:
   - Settings: Setting | Value | Last confirmed
   - People: Name | Relationship | Lives in (for delivery) | Birthday | Birth year | Key dates | Scenes & interests | Stated wishes | Details mined | Avoid | Gift-relevant sensitivities | Last updated
   - Gifts: Date | Person | Occasion | Gift | Cost | Reaction (their words or second-hand) | Quality 1-5 | Feedback source
   - Rejections: Date | Person | Idea | Reason | Note
2. The record is private by design. Never suggest publishing or sharing it.
3. If Drive isn't connected, or writing to cells fails, give the user paste-ready rows for each tab instead.

## Step 1 - Universal settings (always first)
Show the saved settings and ask "Still true?" (Yes / Update). On first run, collect them. Settings are about the gift-giver (the user), never the recipient:
- Definition of a great gift
- Spending comfort right now (relaxed / normal / careful)
- How and where the user shops (online UK, online international, in person locally, a mix), plus their own country for currency and shop choice
- Practical priorities (multi-select): quality and brand, convenience, price, delivery speed, shops where they already have a membership, discount or loyalty scheme (ask which ones), preferred and avoided shops
- Values (multi-select): local and independent, sustainable, handmade or personal, no strong preference
Where a recipient lives is a per-person detail, recorded in People, not a setting.

## Step 2 - The basics (one screen)
- Occasion (birthday / Christmas / anniversary / thank you / get well soon / Other). For get well soon, follow the filters strictly: comfort and cheer, never anything that points at the illness unless the user invites it.
- Person (existing names from People / someone new)
- Timing: "How long until you'll give them the gift?" (a week or more / under a week / a day or two)
- Budget band: show amounts in the user's local currency, using the country saved in Settings (or their location if known), with bands rounded to sensible local amounts. If the currency is unclear, ask once and save it.
Calculate their age from birth year and flag milestone birthdays (e.g. 18, 21, 30, 40, 50, 60, 65, 70, 75, 80+).

## Step 3 - Know the person (new person, or refresh if stale)
Scene-style questions, for example:
- "Their free Saturday, honestly - what are they doing?" Pick 4 options suited to the person from this wider pool: long brunch with friends; out in nature; making something; curled up with a story; at a gallery or museum; out partying; at work (never truly free); busy with family or caring for others.
- "When did you last see them genuinely light up?" Pick 4 from: hearing an old song; somewhere new; being made a fuss of; tasting something great; spotting a fun outfit while shopping; bumping into someone they hadn't seen in years; a lucky find (like money in a coat pocket); looking at old photos.
- People rarely fit four boxes, so keep pools wide, vary the options between runs, and treat any typed answer as the best data of all.
- "Which would they secretly love? Tick all that apply." (fixes a daily annoyance / a reminder of their past / a treat they'd never buy themselves / time with people they love). Multi-select: the best gifts often do more than one job.
- "Is there something they love that has no place to live?" (e.g. photos they can't display at home, a hobby with no space, a collection kept in a box)
- "Where in their day would they see a gift most?" (keys / phone or wallet / desk / car / kitchen / a bag they carry). For busy people, a gift that lives in their routine beats one that waits on a shelf.
- "Have they asked for anything, or is there a gift you've already started?" A stated wish is a serious option, not second best: research shows givers undervalue what was asked for.
- "Have they mentioned anything in passing, complained about something, or searched for something and given up?" Small throwaway remarks often lead to the most remembered gifts.
- "Is there something they've ruled out because of time, money or caring duties?" The gift can remove the obstacle, and the giver's own time (e.g. covering childcare) can be part of it.
Record past gifts with cost, reaction and who reported the reaction.

## Step 4 - Detail-mining (the heart of the skill)
Ask: "Have they ever told you a story about..." (childhood home / a place they long for / a job they were proud of / something they lost / a memory only you two share). Multi-select. Then one short typed follow-up for the strongest ticked item only.

Then dig for the meaning behind the detail with one multiple-choice screen: where it came from (e.g. a gig or festival, a trip abroad, a gift from someone special, a find they bought for themselves at a turning point), and why it mattered (who they were then, a person, a place, a scene or community they belonged to). The object is a clue, not the answer: the gift should speak to the meaning, not replace the thing.

Never narrow the user's answer (e.g. "gig or festival" does not mean "band"): ask which event, place or person it was. If it's well known, look up what it publicly stands for and offer that as a hypothesis, never a fact. Then confirm it through what the giver has observed, not what they know, e.g. "When they talk about it, do they light up, go wistful, or laugh?" and "Do they still keep photos or outfits from it?" Prefer gifts that still work if the hypothesis is slightly wrong. A keepsake's value usually lies in how it made the person feel about themselves, not in the object or its craft, so aim the gift at restoring that feeling now rather than at another artefact from then. If the event's culture conflicts with a saved setting (e.g. a gifting culture that values handmade over branded), say so and let the user choose.

If a loss comes up (a person, a pet, a home), a remembrance gift can be the most meaningful of all, such as a late grandparent's recipes in a box, or a recording of a voice. Don't filter it out and don't assume it: ask the giver gently whether a gift honouring that loss would be welcome now.

## Step 5 - Ideas
1. First propose three genuinely different directions (not three parts of one idea), each tied to the meaning behind a detail from Step 4 or a stated wish. At most one direction may be a literal replacement of something lost; the others should answer what it meant. Look for at least one direction that does more than one job at once (e.g. meaning plus a daily fix, placed where they'll see it every day), as in a keyring carrying a treasured photo for someone who loses their keys and can't display photos at home. Directions need not be products: an experience shared together (which research shows strengthens relationships more than things do) or an act of care (fixing what's broken, preparing for a hard day) are valid directions.
2. Check each against: the user's standards, their practical priorities (prefer shops where they hold a membership or discount, and say when one applies), total cost including hidden costs (travel, childcare), timing and delivery, whether it depends on people who may not cooperate, "Will they still value this in six months?" (givers over-focus on the moment of opening; recipients value lasting use), and whether it suits the occasion's tone: romantic occasions (anniversary, Valentine's) usually call for something personal, so a practical gift there needs a note showing the attention behind it. For food or perishables, check freshness and delivery condition, because a damaged or spoiled gift reads as careless. Say plainly if an idea fails a check.
3. Once a direction is chosen, find real products or bookings with shop links (web search). Never invent a link.

## Filters - never suggest
- Anything that points at a difficulty (e.g. sleep aids for an insomniac, fitness kit for someone struggling with fitness).
- Anything against medical advice the user has mentioned (e.g. alcohol, vaping).
- Anything touching sensitive personal history the user hasn't invited (remembrance gifts are welcome once the giver says so; see Step 4).
- The user's baseline gift (e.g. flowers every visit) presented as the main gift.
- Categories the person has rejected before, or buys for themselves and never uses.
- Anything needing ongoing effort the person dislikes (e.g. garden upkeep).
- Anything that clashes with who they are (e.g. a rival team's merchandise for a loyal fan). The gift must fit their identity, not the giver's.
- Experiences that ignore a known fear or limit (e.g. a helicopter ride for someone with vertigo). Before any experience, ask: "Anything they're afraid of, or physically can't do?"
- Clothes or shoes, unless the giver knows their size and style for certain. These are the most-returned gift category.
- Generic consumables (toiletries, beauty sets, drinks, food hampers) as the main gift. These are the most regifted items. Apply the test: "Could this be for anyone?" If yes, it isn't the gift.
- Cash or vouchers, unless the person asked for them. Otherwise they can read as no thought at all.
Weigh second-hand feedback ("Dad says she liked it") below the person's own words.

## Step 6 - Rejection loop
If the user rejects an idea, ask for a reason (too generic / over budget / they'd hate it / logistics / too sensitive / Other). Log it in Rejections, apply it immediately, and offer new directions. Rejection reasons are the most valuable data the skill collects.

## Step 7 - Close
- Log the chosen gift in Gifts (cost and occasion now; reaction and quality score later).
- Update the person's row with new details mined.
- Offer to draft a short note to go with the gift, saying why the giver chose it, including the story of the hunt if there was one. Words about the person are often what's remembered most.
- Suggest asking the shop for a gift receipt, so a miss is easy to fix without awkwardness.
- Offer to draft any messages needed to make it happen (e.g. booking, asking family).

## Version log
- v1 (Oct 2026): built from a live run for a milestone birthday. Learned: settings first; diverge before converging; scene-style closed questions; detail-mining; feasibility checks; the filters above.
- v1.1 (Oct 2026): prepared for public release. Added "What you need" and a no-Drive fallback; question style works without a dedicated question tool; generalised examples. First test run fixes: settings clearly about the giver, not the recipient; shopping channel includes online; practical priorities (convenience, price, delivery speed, memberships and discounts) added; recipient location moved to People; quality and brand priority; thank-you and get-well-soon occasions; clearer timing question; budget in local currency; wider Step 3 option pools; dig for the meaning behind a detail, not just the object, and limit literal replacements to one direction. Reverse test (studying a real gift that landed) fixes: multi-select "secretly love"; new questions on loves with no place to live and where in their day they'd see it; "looking at old photos" option; at least one multi-job direction. Story study (about 30 published "best gift ever" stories plus gift-giving research) fixes: questions on passing comments and ruled-out wishes; stated wishes prioritised; experience and care directions allowed; gentle remembrance-gift check; a note with every gift; six-month value check. Misses study (UK unwanted-gift, return and regifting surveys, plus disappointed-recipient stories) fixes: new filters for identity clashes, ignored fears, clothing without known size, generic consumables, unrequested cash; occasion-tone and condition checks; gift receipt.

## Ideas for v2
- Birthday reminders via scheduled tasks.
