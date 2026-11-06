# Mode: Focus

When there's already a field or 2–3 candidates (from a previous `explore` or brought by
the user) and it's time to narrow down with real evidence. Active web search. It maps
the competition, dead products and channel reality for each candidate, and narrows
iteratively as the user reacts. Its job: go from "a few candidates" to "the chosen one,"
with grounding.

## Constraints

1. **Every claim about the outside world** (competitor, pricing, demand, channel,
   traction) needs a web source. No source → mark it `[Inference]`.
2. **Mom Test required** when analyzing reviews/signals: discard generic praise,
   prioritize behavior, pain and workarounds (spreadsheets = strong signal).
3. **No number theater.** Market size only with a source. Flag self-reported revenue.
4. **Lean output.** Tables > prose. Target: 2–3 screens.

## The deep-research invitation (a feature of this skill)

Focus is where research depth decides quality. **Right at the start of the mode, assess
whether the task calls for a broad sweep** (mapping competitors, dead products and
channels for several candidates usually does). If it does, **stop and flag it to the
user** before searching:

> "This step gets much stronger with deep research. If you have the extended research
> mode available in your interface, turn it on now and I'll do a broad sweep of
> competitors, dead products and channels for the candidates. If you'd rather not, I'll
> go ahead with normal web search, which covers the essentials with less depth and fewer
> sources. Which do you prefer?"

Notes on this:
- Claude **can't turn on** extended research mode by itself; it's a user control. The
  skill's role is to flag the best moment, not to try to trigger it.
- Normal web search (which Claude runs on its own) handles 6–15 focused searches well.
  Extended research runs dozens and synthesizes; it's better for broad sweeps.
- If the user continues without extended mode, **don't block**: do the normal search and
  name what got less coverage.
- Respect the user's control and the tone of the other skills: offer, name the
  trade-off, don't push.

## Protocol

### Step 1: Confirm the candidates
List the 2–3 candidates going into focus (from explore or from the user). Restate the
founder's profile in one line; the fit is always against it.

### Step 2: Research plan (show before searching)
5–10 concrete questions the research will answer, per candidate. Examples:
1. Who are the 3–5 direct competitors? Traction? Pricing?
2. What are the recurring complaints in reviews/threads?
3. Which products died in this space, and why?
4. What's the real acquisition channel that works here for someone with no audience?
5. Is there a spreadsheet/workaround signal (unmet demand)?
6. Pricing benchmark: does the audience pay?

This plan becomes the backbone of the output. (This is where, or right before where, the
deep-research invitation above comes in.)

### Step 3: Run the searches
Principles: short queries (1–6 words); search for specific competitors, not concepts;
**search for dead products/pivots** (half the learning); search for behavioral reviews
(G2, Product Hunt, Reddit, IH, HN); search pricing pages directly. Apply the Mom Test to
everything.

### Step 4: Competitive map per candidate
| Player | Type | Approach | Pricing | Traction (flag) | Gaps | Source |
|---|---|---|---|---|---|---|
Types: Direct / Indirect / Adjacent / Status quo. The status quo (spreadsheet, nothing)
is often the real competitor.

### Step 5: Channel reality per candidate
The question focus exists to answer with evidence: **given the founder's reach, is this
product discoverable?** Look for real cases of solo founders who grew something similar
starting from zero audience: which channel they used, how long it took, what MRR they
reached (flag self-reported). This feeds Channel Fit with fact, not assumption.

### Step 6: Pre-mortem per candidate (quick)
12 months from now, this one failed. The 3 most likely causes. Feeds the risk and the
score.

### Step 7: Re-score with `fit-rubric.md`
Now with evidence. Scores MUST change from explore if the research revealed something,
Channel Fit and Market Pull especially. Apply the Channel Fit override.

### Step 8: Narrow and decide
Final ranking of the candidates. Recommend the top 1 (or say "it's a tie, and the
tiebreaker is X"). If the user reacts and narrows further, iterate; focus is iterative
by nature.

## Output structure (template)

```
## Focus: [candidates]

*Founder profile (1 line). Fit is always against this.*

### Research plan
[5–10 questions]
[+ deep-research invitation, if applicable]

### Per candidate
**[Candidate A]**
- Competitive map [table]
- Channel reality [fact + source]
- Pre-mortem: [3 causes]
- **Fit Score** [4 components + total + verdict, with override if any]

[repeat per candidate]

### Ranking and recommendation
[top 1 with 3 evidence-grounded reasons; or a tie + tiebreaker]

### Next step
[/market-research on the chosen one, OR pressure-test if the user wants to stress it
before committing, OR back to explore if none passed]
```

## Anti-patterns (don't)
- Don't mark as "fact" what has no source. A marked inference is fine.
- Don't run 30 searches in normal mode with no gain; if you need a broad sweep, that's a
  sign the deep-research invitation should have been made.
- Don't copy competitor marketing as analysis; look for what users say.
- Don't finish without a ranking and a recommendation. A tie is an answer; "needs more
  research" with no verdict isn't.
- Don't leave Channel Fit as an assumption when channel evidence is available.
