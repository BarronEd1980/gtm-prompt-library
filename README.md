# GTM Prompt Library

A curated set of prompts I use in my day-to-day as Director of Partnerships & New Business at eDreams ODIGEO — across B2B sales, partner discovery, deal prep, and platform GTM.

Sharing publicly because (1) the best commercial conversations happen when teams have a shared vocabulary for what "good prompting" looks like, and (2) most prompt libraries online are written by engineers for engineers. This one is written by an operator, for operators.

Tested mostly with **Claude (Sonnet & Opus)** and the **Anthropic API**, but works just as well with ChatGPT or Gemini. Most prompts are zero-shot; a few are templates with `<placeholders>` to fill in.

> Maintained by [Edu Barrón](https://www.linkedin.com/in/barroned). Feedback welcome.

---

## Index

1. [Partner discovery & qualification](#1-partner-discovery--qualification)
2. [Cold outreach to a senior executive](#2-cold-outreach-to-a-senior-executive)
3. [Pitch deck critique](#3-pitch-deck-critique)
4. [RFP / term sheet summarization](#4-rfp--term-sheet-summarization)
5. [Strategic intel brief on a target account](#5-strategic-intel-brief-on-a-target-account)
6. [Internal stakeholder alignment](#6-internal-stakeholder-alignment)
7. [Customer journey storyboarding](#7-customer-journey-storyboarding)
8. [Market sizing — bottoms-up TAM](#8-market-sizing--bottoms-up-tam)
9. [Negotiation prep](#9-negotiation-prep)
10. [30-minute meeting prep brief](#10-30-minute-meeting-prep-brief)

---

## 1. Partner discovery & qualification

**When I use it:** A new partnership lead lands in my pipeline and I need to decide in 15 minutes whether it's worth a discovery call.

````
You are helping me, a B2B partnerships lead, decide whether to pursue
<COMPANY> as a partner for <OUR_PRODUCT>.

Based on the context I paste below, give me:

1. Strategic fit (1–5) — how well their business model and current
   strategy line up with what we offer. One paragraph of reasoning.
2. Top 3 reasons they'd say yes — framed in their language, not ours.
3. Top 3 reasons they'd say no — including the objection I'd find
   hardest to handle.
4. Decision-maker map — who I should target first, and who they
   likely report to.
5. My opening hook — one sentence I'd use to start the conversation,
   anchored on a recent public move they've made.

Be specific and senior-level. Skip generic platitudes.

Context:
<paste annual report / press release / About page / news>
````

**Notes:** Output is only as good as the source. I usually paste the last earnings release plus 3–5 recent press articles.

---

## 2. Cold outreach to a senior executive

**When I use it:** First email to a VP+ at a target partner where I have a clear hook but my first draft sounds like a template.

````
Draft a 3-paragraph cold email from me to <NAME>, <TITLE> at <COMPANY>.

Goal: book a 20-minute exploratory call about <TOPIC>.

Constraints:
- 120 words max total.
- Tone: peer-to-peer, not vendor-to-buyer. Senior, calm, specific.
- No "I hope this finds you well", no "quick question", no
  exclamation marks.
- Open with one specific observation that proves I've done my homework.
- CTA is the last sentence, not a separate paragraph.

Context:
- Hook: <recent funding / launch / org change / interview quote>.
- My specific value to them: <ONE concrete thing>.
- Why I'm credible to send this: <my role / company / shared
  connection>.

Write 3 variants with different opening hooks. Label each.
````

**Notes:** I always rewrite the final version in my own voice. The model gets the structure right; I get the voice right.

---

## 3. Pitch deck critique

**When I use it:** After a first draft of a B2B deck, before I send it to my team for review.

````
You are a skeptical CFO sitting in the back of the room while I
present this pitch. Find what's weak before my audience does.

For each slide I paste below, tell me:

1. Message in 5 seconds — what does a glancing reader take away?
   If unclear, say so.
2. Credibility check — any number, claim, or comparison that would
   make a numerate executive raise an eyebrow.
3. Hidden assumption — what am I assuming the audience already
   believes, that they may not?
4. Cut or keep — is this slide load-bearing, or could I delete it
   and lose nothing?

End with: the one slide I should rebuild from scratch, and why.

<paste slide text / speaker notes>
````

**Notes:** Brutal framing in the prompt = useful output. Polite framings produce polite, useless feedback.

---

## 4. RFP / term sheet summarization

**When I use it:** Inbound RFP or partner-drafted term sheet that's 20+ pages and I have 30 minutes to brief leadership.

````
Summarize the document for an internal 1-pager. Audience: my CFO
and CEO. They have 3 minutes.

Structure:

1. What they're asking for — plain English, no jargon.
2. Commercials — fees, splits, exclusivity, term, termination rights.
3. Hidden constraints — clauses that look standard but would
   actually limit us (MFN, audit rights, data ownership, etc.).
4. What they actually want — the underlying need they're trying
   to solve. Often different from what the document says.
5. My recommendation — pursue / pursue with conditions / decline.
   One paragraph of reasoning.
6. 5 questions I'd ask them in the next call — to surface what's
   not in the document.

<paste document>
````

---

## 5. Strategic intel brief on a target account

**When I use it:** Before a kickoff meeting with a new prospect, when I need to walk in knowing more than my counterpart expects.

````
Build me a 1-page strategic intel brief on <COMPANY>'s
<BUSINESS_LINE>.

Sections:

1. Business model in two sentences — how they make money, in their
   own framing.
2. Last 12 months — most important strategic moves: leadership
   changes, product launches, partnerships, M&A, fundraising.
   Date each one.
3. Public commitments — what they've publicly said they'll do in
   the next 12–24 months. Source each claim.
4. Known weaknesses — areas where competitors or analysts have
   pointed out gaps.
5. My entry angle — three distinct ways <OUR_PRODUCT> connects to
   their current priorities. Rank by likely traction.
6. People to know — the 3–5 names I should look up before the
   meeting, with one-line context each.

Prioritise their 10-K / annual report / earnings calls. Use press
only if recent and credible.
````

**Notes:** Run with web search enabled. Then cross-check dates manually — models still hallucinate timelines occasionally.

---

## 6. Internal stakeholder alignment

**When I use it:** When I need to sell an initiative internally and my first draft is in the wrong language for the audience.

````
I need to sell <INITIATIVE> to <INTERNAL_STAKEHOLDER>
(e.g. CFO / Head of Product / Legal).

Their incentives: <what they're measured on>.
Their typical objections: <historical pattern>.

Rewrite my pitch in their language:

1. Lead with the metric or risk they care about most.
2. Frame the proposal as solving a problem they already
   acknowledge — not introducing a new one.
3. Make the ask small enough that "yes" is easier than "no".
4. End with what specifically I need from them in the next 7 days.

My current draft:
<paste>
````

---

## 7. Customer journey storyboarding

**When I use it:** Mid-pitch, when I need to make an abstract value prop emotionally concrete for the audience.

````
Build a customer journey storyboard for <PERSONA> using <PRODUCT>
for <USE_CASE>.

5 scenes. Each scene has:

- Setting — where they are, what time of day, what they're trying to do.
- Emotion — one specific feeling, named. "Frustrated" is fine.
  "Quietly anxious because the booking is for her parents" is better.
- Product touchpoint — the one thing our product does in this moment.
- Business value — the metric this scene moves for the partner
  (conversion, retention, NPS, ancillary attach).

Tone: cinematic but plausible. No fairy tales.

End with: the one scene I should cut if I only have 3 minutes to
present, and why the other 4 are stronger.
````

---

## 8. Market sizing — bottoms-up TAM

**When I use it:** When a partner asks "how big is this opportunity for us, really?" and "trust me" isn't an answer.

````
Help me size the addressable opportunity for <PRODUCT> in <MARKET>,
bottoms-up.

Step 1 — define the buyer. Who specifically would adopt this? Be narrow.
Step 2 — estimate units. How many of those buyers exist? Source it.
Step 3 — estimate spend / value per unit per year. Range, not point.
Step 4 — calculate the band (low / mid / high).
Step 5 — sanity check against a top-down number (e.g. analyst report).
   If they diverge by more than 2x, flag where the gap is.
Step 6 — list the three assumptions most likely to be wrong, and
   what would change the answer.

Show your working. I'd rather defend a transparent estimate than a
precise black box.
````

---

## 9. Negotiation prep

**When I use it:** The night before a serious negotiation.

````
I'm negotiating <DEAL_TYPE> with <COUNTERPARTY>.

Give me:

1. Their BATNA — what they walk away to. Realistic, not flattering.
2. My BATNA — what I walk away to. Honest, including the cost of
   walking.
3. 5 likely demands they'll open with — ranked by probability.
4. My pre-prepared response for each — short, specific, not defensive.
5. The one trade I should be willing to make — what I'd give up,
   what I'd get in return, and the threshold at which I'd actually
   do it.
6. The thing they might ask for that I should absolutely not concede,
   and the reframe I'll use if they push.

Context:
<paste>
````

**Notes:** Probably the prompt I rerun the most. I've stopped going into negotiations without it.

---

## 10. 30-minute meeting prep brief

**When I use it:** Next meeting in 30 minutes and I want to walk in calibrated, not improvising.

````
I have a meeting with <NAME>, <ROLE> at <COMPANY> in 30 minutes.
Stated agenda: <agenda>.

Give me:

1. What's likely top-of-mind for them this week — based on their
   company's current public situation.
2. 3 questions I should ask — one to learn, one to qualify, one to
   advance the relationship.
3. What success looks like for this meeting — a single specific
   outcome, not "good conversation".
4. The one thing I should NOT say — based on what could damage
   trust or close doors prematurely.
5. My opening line — first 20 seconds, in the tone of a peer, not
   a vendor.

Context:
<paste recent news / their LinkedIn / our prior history>
````

---

## License

Use anything here freely. Attribution appreciated, not required.

