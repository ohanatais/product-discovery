# Fit Rubric

This skill's rubric doesn't score the **idea**; it scores the **fit** between founder,
market and channel. That's what sets it apart from `idea-validation` (which scores an
idea that's already been chosen). Four components, 0–25 each, total 100. Always
**justify the score** in 1–2 sentences; never give a bare number.

The golden rule: the same idea has different fits for different founders. An idea that
scores 22 on Market Pull and 6 on Channel Fit **is not a good opportunity for this
founder**; it's a trap. The rubric exists to expose that trap, not to hide it behind a
high average.

## 1. Founder Fit (0–25)

Does the founder have a real unfair advantage here, and does it teach them what they
want to learn?

- **0–5**: No advantage at all. The founder comes in like any stranger. It teaches
  nothing they want to learn.
- **6–10**: Genuine interest, but a weak or generic advantage. A long learning curve
  before any differentiator.
- **11–15**: Some relevant expertise or access. It teaches something useful, but the
  founder's edge isn't clearly better than an average competitor's.
- **16–20**: A real unfair advantage (domain, skill, lived experience) that few people
  have. Building this develops exactly the skill the founder wants.
- **21–25**: A strong AND rare AND hard-to-copy unfair advantage, in a space where the
  founder plays on home turf. The project is simultaneously the product, the portfolio
  and the course they wanted to take.

**Signals to look for:** has the founder done this before? Do they have access others
don't (community, data, network, domain experience)? Is what they'd learn building this
what they said they want to learn? Watch out for "imagined advantage": interest is not
advantage.

## 2. Channel Fit (0–25) — the decisive axis

Given the founder's REAL reach today, can this product be discovered through them? Most
ideas die here, not on the merit of the idea.

- **0–5**: The only distribution path is one the founder doesn't have and can't build
  (e.g., it requires a large audience they don't have, or sales they won't do).
  "Build it and they'll come."
- **6–10**: The channel exists but is hostile to the founder's profile (e.g., it
  requires cold outbound from someone who hates selling, or YouTube from someone who
  won't make videos). High friction, slow to compound.
- **11–15**: A plausible channel compatible with the founder's temperament, but no
  distribution advantage: they compete for attention on equal footing with everyone.
- **16–20**: A clear channel, compatible with what the founder is willing to do, with
  some compounding engine (SEO, content, community, free tool, teardown loop).
  Discoverable without a pre-existing audience.
- **21–25**: A channel where the founder has a specific distribution advantage: a
  community they're already in, a content angle that plays to their strength, a loop
  where building the product ALREADY is the marketing. Distribution and product
  reinforce each other.

**Signals to look for:** what is the CONCRETE channel (not "marketing")? Can this
specific founder work it today, with the reach and temperament they have? Does it
compound (every effort leaves an asset) or is it rented (stop, and it dies)? **If the
best channel requires something the founder said they won't do, the score is low, no
exceptions.**

## 3. Market Pull (0–25)

Is there real pain, frequent and costly enough, in a space with people to reach and not
so saturated that it smothers a solo entrant?

- **0–5**: A solution looking for a problem. No sign of pain. "Would be nice to have."
- **6–10**: Mild or sporadic pain; or a market so saturated there's no opening for a
  solo entrant (a red ocean with well-funded incumbents at parity).
- **11–15**: Recurring pain in an identifiable niche, with visible workarounds
  (spreadsheets, hacks). The space is occupied but a wedge is possible.
- **16–20**: Frequent, costly pain, people already paying for partial solutions, and an
  unsaturated entry angle (niche, language, underserved audience).
- **21–25**: Acute pain validated by active use of inadequate alternatives, a community
  complaining publicly, proven spend, AND the space has a clear gap that incumbents
  don't cover because of their own structural constraints.

**Signals to look for:** negative reviews of adjacent products, complaint threads,
spreadsheets as the real competitor, dead products (why did they die?), signaled
willingness to pay. Apply the Mom Test: behavior > opinion.

## 4. Build & Monetize Fit (0–25)

Can an excellent, focused MVP be built solo, with an operating cost compatible with what
can be charged?

- **0–5**: Requires tech/capital/a team the founder doesn't have; OR negative unit
  economics (e.g., heavy LLM inference per free user); OR an audience with no
  willingness to pay.
- **6–10**: Buildable but complex (6+ months solo) or distant monetization (needs to
  scale a lot before earning). Tight margin.
- **11–15**: A focused MVP in 1–2 months solo with a known stack; a plausible revenue
  model (freemium, SaaS, info-product) but unvalidated pricing.
- **16–20**: An excellent MVP in weeks, low tooling cost, and a pricing benchmark exists
  in similar products with an audience that pays. Healthy margin early.
- **21–25**: Buildable and polishable fast with off-the-shelf/AI-assisted tools, near-zero
  marginal cost, and multiple revenue paths (e.g., info-product + tool) with WTP already
  demonstrated in the space.

**For solo projects / vibe coding:** this component weighs more. Consider inference
cost, maintenance complexity, and whether doing it REALLY well is feasible alone.
Focused simplicity is worth more than broad scope.

## Aggregate and mapping to Verdict

Sum of the 4 components (0–100).

| Score | Verdict |
|---|---|
| 0–39 | **PASS** (don't pursue; the fit isn't here) |
| 40–64 | **EXPLORE FURTHER** (partial fit; narrow or reframe before committing) |
| 65–100 | **PURSUE** (strong fit; take it to `/market-research` and validate) |

**For a personal / side project**, the `PURSUE` threshold drops to **≥ 58**, but this
must be stated explicitly in the output, because it deliberately lowers the bar.

## Mandatory override (the rule that defines the skill)

**If Channel Fit ≤ 8, the maximum verdict is EXPLORE FURTHER, regardless of the
aggregate.** An idea with Market Pull 24, Founder Fit 22, Build 20 and Channel Fit 6
adds up to 72, but it's a trap: an excellent product nobody will discover. In that case
the verdict is EXPLORE FURTHER with the explicit recommendation: "the bottleneck is
distribution, not the idea. Either solve the channel or pick another opportunity."
Every override must be explained.

The classic override also applies: if any component is catastrophic (≤ 4) in a context
that makes it fatal, the verdict can be PASS even with a higher aggregate.

## Score output format

```
**Fit Score — [opportunity name]:**
- Founder Fit: 19/25 — [1-sentence justification]
- Channel Fit: 21/25 — [1-sentence justification]
- Market Pull: 16/25 — [1-sentence justification]
- Build & Monetize Fit: 18/25 — [1-sentence justification]
- **Total: 74/100 — PURSUE**

[If there's an override, state it here and explain.]
```

## A note on ranking several

In `explore` mode, score quickly and comparably (one line per component) for 8–12
opportunities in a table, and go deeper on the rationale only for the top 3–4. In
`focus`, score the 2–3 candidates in depth with web evidence. In `pressure-test`,
re-score the single candidate after attacking the three axes; the score should change if
the attack revealed something. A score that doesn't move after an honest pressure-test
is a sign the test was weak.
