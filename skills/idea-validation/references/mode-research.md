# Mode: Research

Analysis with active web search. Every market claim has a source. Focus: produce a grounded verdict, not a pretty report.

## Constraints

1. **Every claim about the outside world** (competitor, pricing, demand, reviews, churn) needs a web citation. No source → mark it `[Inference]`.
2. **Mom Test required** when analyzing reviews: discard generic praise, prioritize behavior and pain.
3. **No number theater**: TAM/SAM/SOM only with a direct source. If there isn't one, say "not available with confidence."
4. **Hard search budget: 6-10 queries.** Each search has a clear question it answers. Above 10 only with an explicit flag to the user. Principle: more searching doesn't make up for it; better to synthesize what you have well.
5. **Lean output.** Tables > prose. Don't repeat what's already clear. Target: 2-3 screens of reading.

## Protocol

### Step 1: Restate the idea in 1 sentence
(Same as quick mode — `references/mode-quick.md`, step 1.)

### Step 2: Research plan (show the user before searching)

List 5-10 concrete questions the research will try to answer. Examples:

1. Who are the 3-5 direct competitors? How many users do they have?
2. What are the most frequent complaints in reviews?
3. What's the pricing benchmark for similar products?
4. Are there signs of churn or pivots among incumbents?
5. What's the size/dynamic of the target niche?
6. Are there dead products in the space? Why did they die?
7. What regulatory/tech trends affect this?

This plan becomes the backbone of the report.

### Step 3: Run the searches

Search principles:

- **Short queries**, 1-6 words, no special operators.
- **Search for specific competitors**, not vague concepts. "Reflect notes review" > "AI note taking apps".
- **Search for churn/pivots/deaths of products** in the space. Learning from the dead is half the work.
- **Search for reviews in sources of real behavior**: G2, Product Hunt, Reddit, recent App Store reviews.
- **Search pricing pages** directly when relevant.

### Step 4: Competitive mapping

Structure (adapted from Anthropic's official framework, simplified):

**Direct competitors:** same problem, same audience, same approach.
**Indirect competitors:** same problem, different approach.
**Adjacent competitors:** could enter the space tomorrow (Notion AI, ChatGPT custom GPTs, etc.).
**Status quo / non-consumption:** what people do today (spreadsheet, paper, nothing).

For each relevant competitor (3-7 in total):

| Competitor | Approach | Pricing | Positive signals | Negative signals | Source |
|---|---|---|---|---|---|

Positive signals = signs of real traction (not marketing).
Negative signals = user complaints, churn, structural problems.

### Step 5: Real demand analysis

Don't trust an abstract "growing market." Look for:

- **Reviews of adjacent products** where users ask for what your idea offers. Quote with source.
- **Reddit/HN/Twitter threads** about the pain. Quote.
- **Search volume signals** (if you can find indications).
- **Existing paid communities** in the space (a WTP signal).

Apply the Mom Test: separate opinion ("would love this") from behavior ("I pay $20/month for X, which doesn't solve Y").

### Step 6: Technical feasibility analysis

Focus on:

- External APIs/services needed and their cost (especially LLM, vector DB, etc.).
- Specific technical risks (accuracy, latency, cost per user).
- Compare with how competitors solved similar problems.

### Step 7: Monetization analysis

- Pricing benchmark with sources (competitors' pricing pages).
- Viable models (SaaS, freemium, one-time, etc.).
- Unit economics if they can be estimated with anchors.
- For a personal project: mark N/A if applicable.

### Step 8: Pre-mortem (5 min)

Imagine the project has failed 12 months from now. List the 3 most likely causes. This exercise feeds the risk register.

### Step 9: Score + Verdict + Risk register + Questions

Score with `scoring-rubric.md`.
Risk register required, 5-7 rows in research mode.
Verdict with 3 grounded reasons (each referencing evidence from the research).

Top 3 remaining critical questions:

- What **still** can't be known without interviewing real users?
- Which hypotheses need testing before any big commitment?
- Which additional kill criteria should be monitored?

## Output structure (template)

```
## Research Validation: [Idea name]

**In one sentence:** [structured rewrite]

### Research plan
[5-10 questions guiding the investigation]

### Competitive mapping
[table]

### Real demand
**Facts:**
- [claim with source]
- [claim with source]

**Inferences:**
- [my read]

### Technical feasibility
[analysis]

### Monetization
[analysis + pricing benchmark with sources]

### Pre-mortem: the 3 most likely causes of failure
1. ...
2. ...
3. ...

### Score
[components + total + rationale per component]

### Risk Register
[5-7 row table]

### Verdict: [BUILD | VALIDATE FIRST | KILL]
1. [reason referencing the evidence]
2. ...
3. ...

### Top 3 remaining critical questions
1. ...
2. ...
3. ...

### Pivot Paths (if Verdict = KILL or score < 55)
**Pivot 1: [short name]**
- Improves: [which score component]
- Why: [reason anchored in the research]
- Trade-off: [what's lost]

**Pivot 2: [short name]**
- ...

(List 2-3. Skip this section if Verdict = BUILD, or VALIDATE FIRST with score ≥ 55.)

### Suggested validation plan (if Verdict = VALIDATE FIRST or BUILD)
[3-5 concrete actions: interviews, landing page test, pretotype, etc.]
```

## Anti-patterns (don't)

- Don't write something unsourced and label it a fact. A marked inference is fine; an unsourced "fact" is forbidden.
- Don't run 30 searches. More than 15 with no marginal gain is waste; better to ask the user for direction.
- Don't copy competitors' marketing as if it were analysis. Look for what users say, not what sellers say.
- Don't end with "interesting, but needs more research" without a verdict. A verdict is mandatory.
