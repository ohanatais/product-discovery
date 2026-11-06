# Mode: Deliverable

`research` mode + formatting for an external audience. The output is meant for a client, stakeholder, investor or another PM, not for yourself.

## When to use

- A PM taking an analysis to a client.
- A portfolio decision in a committee.
- Evaluating a proposal from an external stakeholder.
- A document that will be read by someone who didn't follow the conversation.

## Constraints

1. **Everything from research mode applies** (every claim sourced, Mom Test, no number theater).
2. **Language adjusted to the audience**: less first person, more neutral/professional voice.
3. **Executive Summary required** at the top (not at the end).
4. **Appendices** with the raw research data (links, quotes, full tables) at the end.
5. **Honest but professional tone**: quick mode's adversarial stance becomes "grounded critical analysis."

## Protocol

Run the full `research` mode protocol (`references/mode-research.md`), and add:

### Step 0: Confirm audience and context

Before producing the output, ask (or infer if obvious):

1. Who is this document for? (client, investor, internal committee)
2. What decision needs to be made based on it?
3. Are there length or format constraints?
4. Which channel will the document be shared through? (email, deck, shared doc)

### Final step: Reformat as a deliverable

Output structure:

```
# Feasibility Analysis: [Product/idea name]

**Prepared by:** [PM]
**Date:** [date]
**Decision supported:** [which decision this document supports]

## Executive Summary

[3-5 paragraphs]
- Clear recommendation: BUILD / VALIDATE FIRST / KILL
- Aggregate score
- Top 3 reasons
- Suggested next steps

## 1. Context and Idea

[1-sentence rewrite + structured description]

## 2. Competitive Mapping

[Professionally formatted table]

## 3. Demand Analysis

[Facts with sources in footnotes or inline links]

## 4. Technical Feasibility

[Analysis]

## 5. Monetization and Business Model

[Analysis + benchmark]

## 6. Risk Register

[Formal table with Impact × Likelihood × Mitigation × Suggested owner]

## 7. Score and Rationale

[Components + total]

## 8. Recommendation

[Verdict with 3 grounded reasons]

## 9. Validation Plan / Next Steps

[Concrete actions with suggested owner and deadline]

## 10. Alternative Paths (if applicable)

[Pivot Paths: 2-3 reframings of the idea if the Verdict is KILL or the score is low. Each with: expected improvement, market grounding, trade-off. Skip if Verdict = BUILD with a strong score.]

## 11. Remaining Critical Questions

[Numbered list]

## Appendices

### A. Sources consulted
[List with links]

### B. Reviews and quotes analyzed
[Relevant quotes with source]

### C. Detailed pricing benchmark
[Full table]
```

## Formatting notes

- **No first person** ("I think," "my read"); use "the analysis suggests," "the evidence indicates."
- **No slang or explicit adversarial stance**; keep the rigor without sounding combative.
- **Honesty preserved**: if the verdict is KILL, the document says KILL. Only the packaging changes, not the substance.
- Appendices can be long; the main body should fit in 2-4 pages.

## Anti-patterns (don't)

- Don't soften the verdict to please the audience. A verdict is a verdict.
- Don't pad with decorative charts or empty sections to look robust.
- Don't hide the analysis's limitations. If the evidence is weak somewhere, say so.
- Don't use unanchored buzzwords ("disruption," "innovation," "transformation" with no operational definition).
