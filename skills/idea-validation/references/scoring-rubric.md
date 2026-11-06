# Scoring Rubric

Rubric for the 4 score components. Each component goes from 0 to 25 (total 100). Always **justify the score** in 1-2 sentences; never give a bare number.

## 1. Demand (0-25)

Is there real pain, frequent and costly enough to change behavior?

- **0-5**: A solution looking for a problem. No sign of pain. "Would be nice to have."
- **6-10**: The pain exists but is mild or sporadic. Users live with it.
- **11-15**: Recurring pain in an identified niche. Visible workarounds (spreadsheets, hacks, apps open side by side).
- **16-20**: Frequent, costly pain, with people already paying for partial solutions.
- **21-25**: Acute pain, validated by active use of inadequate alternatives, a community complaining publicly, proven spend.

**Signals to look for:** negative reviews of adjacent products ("I wish Notion did X"), forum/Reddit threads, signaled willingness to pay, frequency of use of alternatives.

## 2. Differentiation (0-25)

Does the idea have defensible differentiation vs. what exists, or is it just "one more"?

- **0-5**: Replicates an existing product with no new angle. Late mover with no advantage.
- **6-10**: Small improvement on an existing product. Easy for incumbents to copy.
- **11-15**: New angle (audience, UX, integration) but weak defensibility.
- **16-20**: Real differentiator (tech, data, distribution) with some early moat.
- **21-25**: Clear wedge + a path to defensibility (network effects, proprietary data, high switching cost).

**Signals to look for:** what could incumbents (Notion, ChatGPT, etc.) add as a feature in 1 sprint? If they could, score low. Is there a market insight others don't have?

## 3. Feasibility (0-25)

Can an MVP that delivers value be built with the resources available?

- **0-5**: Requires tech that doesn't exist, or a team/capital the user doesn't have.
- **6-10**: The tech exists but integration is complex. MVP takes 6+ months solo.
- **11-15**: MVP feasible in 2-3 months solo with a known stack. Medium technical risks.
- **16-20**: MVP in weeks, mature stack, low technical risks.
- **21-25**: MVP in days/a few weeks, off-the-shelf tools, low-code/no-code viable.

**For vibe coding/solo projects:** this dimension weighs more. Consider API availability, LLM inference cost, maintenance complexity.

## 4. Monetization (0-25)

Is there a plausible path to revenue that covers the cost of operating?

- **0-5**: Audience with no willingness to pay, high unit cost (e.g., heavy LLM inference per free user).
- **6-10**: Monetization possible but distant (needs to scale a lot first).
- **11-15**: Plausible model (freemium, SaaS) but pricing not validated.
- **16-20**: Pricing benchmarks exist in similar products, the audience pays.
- **21-25**: Proven WTP, positive unit economics early on, multiple viable models.

**For a personal project with no commercial goal:** mark it **N/A** and don't add it to the score. The total in that case is out of 75. State this explicitly.

## Aggregate

Sum of the 4 (or the 3, if monetization is N/A).

## Mapping to Verdict

| Score (out of 100) | Verdict |
|---|---|
| 0-39 | **KILL** |
| 40-64 | **VALIDATE FIRST** |
| 65-100 | **BUILD** |

| Score (out of 75, personal project) | Verdict |
|---|---|
| 0-29 | **KILL** |
| 30-48 | **VALIDATE FIRST** |
| 49-75 | **BUILD** |

**Override allowed:** if a single component is catastrophic (e.g., Differentiation = 2 in a saturated market), the verdict can be KILL even with a higher aggregate. The override must be explained.

## Score output format

```
**Score:**
- Demand: 18/25 — [1-sentence justification]
- Differentiation: 9/25 — [1-sentence justification]
- Feasibility: 20/25 — [1-sentence justification]
- Monetization: 12/25 — [1-sentence justification]
- **Total: 59/100**

**Verdict: VALIDATE FIRST**
1. [Reason 1]
2. [Reason 2]
3. [Reason 3]
```
