# Guide: Product Discovery Before You Code

> This guide is meant to be read inside Claude Code, or in any Markdown reader.
> Each module takes 20 to 60 minutes. You can stop and pick up where you left off.

---

## Why this guide exists

Most "build with AI" tutorials start at the code.

You install Claude Code, watch a 10-minute video, and start building. A week later you have an MVP running. Two months later you realize you built the right thing for the wrong people, or the wrong thing for everyone.

This guide exists for what comes before that.

It's not about installing tools. It's about the questions that, answered before the first line of code, completely change what you build, and whether it's worth building at all.

---

## What you'll learn

Each module covers one stage of the product journey. The order matters: each answer informs the next question.

| Module | Core question | Skill |
|---|---|---|
| [1. Market research](#module-1-market-research) | Does the market exist? Who else is here? | `/market-research` |
| [2. Idea validation](#module-2-idea-validation) | Is this idea worth the effort of building? | `/validate-idea` |
| [3. Personas](#module-3-personas) | Who exactly am I building for? | `/personas` |
| [4. Positioning](#module-4-positioning) | Why would someone choose this over everything else? | `/positioning` |
| [5. PRD](#module-5-prd) | What exactly am I building first? | `/prd` |

You don't need the skills to follow the guides. But the skills do the work with you, inside Claude Code, in whatever language you speak.

---

## How to use this guide

**If you're starting from scratch:** follow the modules in order. Each has a reading section (~10 min) and a practice section (~20–40 min with the matching skill).

**If you're already midway through:** jump to the module you're on. But if something feels confusing downstream, the answer is almost always in a step you skipped upstream.

**If you only want the skills:** each module has install and usage instructions for the matching skill. You don't need to read the whole guide.

---

## Module 1: Market research

### What it is and why it matters

Market research isn't about confirming your idea is good. It's about understanding the terrain before committing to it.

When you research a market, you're answering three questions:

1. **Who else is here?** Direct, indirect and adjacent competitors, and the status quo (what people do today with no tool at all)
2. **Is the space crowded, or is there room?** Red ocean vs. blue ocean, and whether there's a niche that hasn't been served well yet
3. **Does the market exist?** Is there evidence that people are actively looking for a solution to this problem, or is it a problem you assumed exists?

### The most common mistake

Most people research to confirm what they already believe. They look for data that supports the idea, ignore what contradicts it, and conclude the market exists because they found a few people with the problem.

The goal of research is the opposite: find the evidence that would kill the idea. If you research honestly and it survives, you have something.

### Red ocean vs. blue ocean

**Red ocean:** many competitors fighting for the same customers with similar products. Competition is fierce because everyone is in the same space.

**Blue ocean:** a space with real opportunity: an underserved audience, an unmet need, or a combination nobody has tried yet.

Most products sit somewhere between the two. The useful question isn't "red or blue?" but "is there a specific niche where this product would have a clear advantage over everything that exists?"

### What to do now

Install the market research skill and run `/market-research` with a description of your idea.

```bash
# Copy it into your project
cp -r path/to/product-discovery/skills/market-research .claude/skills/

# In Claude Code:
/market-research
```

The skill will ask how familiar you are with market research and adapt the depth of the analysis. If it's your first time: guided mode, with each step explained. If you already know what you want: it goes straight to the analysis.

**What you'll have at the end:** a map of who's in the space, an honest market sizing (TAM/SAM/SOM), an ocean read, and a clear strategic implication.

---

## Module 2: Idea validation

### What it is and why it matters

Market research maps the terrain. Idea validation tests whether your specific idea fits that terrain.

They're different things. A large market with proven demand doesn't mean *your version* of the product will work. Validation is about finding the riskiest assumption under the idea, the one that changes everything if it's wrong, and testing it before you build.

### The difference between validation and feedback

"I showed it to five people and they all loved it."

That's not validation. People are polite. Friends and family even more so. They tell you what you want to hear, especially when you're excited.

Real validation looks like behavior: someone paid for something similar. Someone built a workaround to solve it. Someone complained about this exact problem in a forum, without knowing you were listening.

Opinion is weak. Behavior is strong. (That's the essence of Rob Fitzpatrick's *The Mom Test*.)

### What the Mom Test is

The Mom Test is a way of asking questions that reveals real behavior, not polite opinions.

The core rule: never ask what people *would* do; ask what they *did*.

- ❌ "Would you use an app that does X?"
- ✅ "How do you deal with X today? Tell me about a recent time."

The second question reveals what the person actually does, how much the problem hurts, and what they consider "good enough" today.

### What to do now

```bash
cp -r path/to/product-discovery/skills/idea-validation .claude/skills/

# In Claude Code:
/validate-idea
```

The skill has three modes: **quick** (initial reaction with no web research), **research** (analysis with searches and sources), and **deliverable** (output formatted for stakeholders).

If you've already done market research: share those documents at the start of the session. The skill will use them as evidence instead of repeating what's been done.

**What you'll have at the end:** a 0–100 score across four dimensions (demand, differentiation, feasibility, monetization), a verdict (Build / Validate First / Kill), a risk register, and, if the verdict is negative, concrete pivot paths.

---

## Module 3: Personas

### What it is and why it matters

A persona isn't a profile card. It isn't "woman, 28, PM in São Paulo, likes productivity."

That doesn't inform a single product decision.

A useful persona answers: **what job is this person trying to get done, and what would make them change their current behavior to use something new?**

That's the difference between building for an archetype and building for a behavior.

### The JTBD (Jobs to Be Done) framework

Jobs to Be Done is a way of understanding why people "hire" products: not who they are demographically, but what progress they're trying to make.

The job statement format: **"When [situation], I want to [motivation], so I can [outcome]."**

- ❌ "I want a better notes app."
- ✅ "When it's the end of the quarter and I need to justify my work to my manager, I want an organized record of what I did with real context, so I don't spend 3 hours piecing it together from scratch and I look more prepared than I feel."

The second is a job statement. The first is a product category.

### The trigger moment

The most important element of a persona isn't the profile; it's the trigger moment.

The trigger moment is the specific event (not a feeling, an event) that moves someone from "this is annoying" to "I need to find a solution now."

Without the trigger, you don't know when your user is ready to be reached or what makes them act.

### What the workaround reveals

What the person does today, without your product, is your real competition.

Not Notion. Not the category leader. The specific spreadsheet they built, the WhatsApp group where they jot things down, or the decision to just not solve the problem.

The workaround shows how much the problem hurts (they're already putting in extra effort), the switching cost (the more elaborate it is, the harder it is to change), and the "good enough" benchmark.

### What to do now

```bash
cp -r path/to/product-discovery/skills/personas .claude/skills/

# In Claude Code:
/personas
```

The skill detects what you have: if you have interviews or real user data → behavioral mode. If you only have hypotheses → hypothesis mode (which makes your assumptions explicit and testable). If it's your first time → guided mode.

**What you'll have at the end:** 1–3 personas with a job statement, trigger moment, current workaround, behavioral (not generic) pains, and, for every assumption without evidence, a note on what would need to be validated.

---

## Module 4: Positioning

### What it is and why it matters

Positioning isn't a tagline. It isn't a mission. It isn't a feature list.

It's the answer to: in a world where these alternatives exist, why would someone who deeply cares about [this specific value] choose this product?

Without a clear answer, your copy will sound generic, your landing page will look like ten others, and your first users will sign up without understanding what makes the product different.

### The Dunford framework (five components)

April Dunford, in *Obviously Awesome*, defines positioning in five components, always in this order:

```
1. Competitive alternatives  →  What does the customer use if this doesn't exist?
2. Unique attributes         →  What does this product have that the alternatives don't?
3. Value                     →  What do those attributes mean for the customer's life?
4. Ideal customers           →  Who cares most about that specific value?
5. Market category           →  Which frame makes that value obvious?
```

The order is non-negotiable. Each component depends on the previous one. Skip one and the positioning falls apart.

### The "so what?" question

After every unique attribute, always ask: "so what? What does this mean for the customer's life?"

Only when you reach an answer that makes someone think "yes, that's exactly what I need" have you found the value.

- Attribute: "Works offline"
- So what? → "You don't lose work when the connection drops"
- So what? → "You can work on a plane, in a basement, in a rural area without anxiety"
- Value: "Reliability that doesn't depend on your connection"

The value is what the customer buys. The attribute is what the engineer builds.

### Pre-PMF: a wide net, not a tuna net

Dunford is explicit: before product-market fit, keep your positioning **loose, like a wide net**. Don't specialize before you see real patterns of who loves the product and why.

The positioning you produce here is a thesis: your best hypothesis given the evidence you have. It isn't a final statement.

### What to do now

```bash
cp -r path/to/product-discovery/skills/positioning .claude/skills/

# In Claude Code:
/positioning
```

The skill has three modes: **guided** (first time, explains each component), **canvas** (you have personas and research and want the canvas directly), and **stress-test** (you have existing positioning and want to find its weaknesses).

**What you'll have at the end:** a filled-in five-component canvas, a positioning statement (for internal alignment, not marketing), what the positioning rules out, and the open questions that would change everything if answered differently.

---

## Module 5: PRD

### What it is and why it matters

The PRD (Product Requirements Document) answers: what exactly am I building, for whom, and why does this version (and not another) make sense to build first?

For a solo builder, the PRD does more than document: it **contains scope**. Every feature you add to the MVP is a week of building you won't get back. Every feature you defer is a week of learning you might gain.

### The solo builder PRD vs. the corporate PRD

They're not the same document.

The corporate PRD has 9+ sections, user journeys, epics, a glossary, and gets published on Confluence to align teams of 20.

The solo builder PRD has 4 sections, fits on a single page, lives in the repository as a `.md`, and is read by Claude Code at the start of every build session.

### The four sections, always all four

1. **Problem**: who has it, what triggers it, what the person does today
2. **Solution**: what the product does, for whom, and why this version
3. **MVP scope**: exactly what's in, observable by the user, with no technical detail
4. **Out of scope**: exactly what's not in this version, with a reason

Section 4 is mandatory. A PRD without an explicit out-of-scope is an invitation to build everything.

### The PRD as Claude Code context

At the start of every build session:

> "Here's the project PRD: [paste the PRD]. Today we're building [capability X from section 3]. [Item Y from section 4] is explicitly out of scope."

This keeps Claude Code from adding features you didn't ask for, making architectural decisions by assumption, or building a version that doesn't match the validated scope.

### What to do now

```bash
cp -r path/to/product-discovery/skills/prd .claude/skills/

# In Claude Code:
/prd
```

The skill checks what you already have (personas, positioning, validation) and uses it as a foundation. If you have nothing, it asks a single question: "Tell me in 2–3 sentences: who it's for, what the problem is, and what the MVP does."

**What you'll have at the end:** a 4-section PRD, ready to use as context in every build session with Claude Code.

---

## Next steps

With the PRD ready, you have everything you need to start building in an informed way.

What comes after this repository:

- **[build-with-claude](https://github.com/ohanatais/build-with-claude)**: Claude Code for non-technical builders, with every technical decision explained, step-by-step tool setup, and how to work feature by feature
- **[brand-and-copy](https://github.com/ohanatais/brand-and-copy)**: visual identity, tone of voice, product copy
- **[go-to-market](https://github.com/ohanatais/go-to-market)**: launch strategy, channels, first users

---

*Made by [Ohana Taís](https://github.com/ohanatais), Senior PM, building in public.*
*Part of the [build-from-zero](https://github.com/ohanatais/build-from-zero) ecosystem.*
