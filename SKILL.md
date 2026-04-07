---
name: groundhog-loop
description: Assess narrative prose, story plans, lorebook.md files, screenplays, or any narrative document against Essence of Groundhog principles — producing a scored assessment with prioritised alignment instructions for stories using extraordinary premises (time loops, body swaps, repeating days, trapped-premise scenarios) as character-driven fables, not genre exercises. Triggers on "groundhog-loop", "groundhog assessment", "essence of groundhog", "assess my loop narrative", "is my story too sci-fi", "genre contamination", "align with groundhog principles", "fable not genre", "premise as weather", "behavioural arc assessment", or when a user submits any narrative involving loops, repetition, extraordinary conditions, or trapped-premise stories and wants to strengthen the human story over the mechanism. Also trigger when the user is writing a story where a character is trapped in an extraordinary condition and wants transformation focus over explanation.
---

# Groundhog Loop — Narrative Assessment Skill

Assess and align narrative works with the **Essence of Groundhog** principles: a behavioural ruleset derived from the structural architecture of *Groundhog Day* (1993) for stories that use extraordinary premises to explore ordinary human transformation — without any reliance on science fiction, guides, explanations, or marked resolutions.

## Before You Begin

Read the grounding document at `references/ESSENCE-of-GROUNDHOG.md` before every assessment. It is the authoritative source for all dimensions and generation rules. Do not work from memory — the document contains specific nuances that matter.

---

## Three Modes of Operation

### Mode 1 — ASSESS (narrative prose or screenplay)

The user provides finished or draft prose, screenplay pages, or a chapter. Assess alignment with each dimension.

### Mode 2 — PLAN (story outline or plot summary)

The user provides a story plan, beat sheet, synopsis, or outline. Assess structural alignment and flag where the plan is likely to produce violations when written.

### Mode 3 — WORLD (lorebook.md or world definition)

The user provides a lorebook, world bible, setting document, or character roster. Assess whether the world architecture supports or undermines the principles — particularly whether the world contains built-in explanation systems, guide characters, or genre scaffolding that would contaminate any narrative set within it.

---

## Assessment Process

### Step 1 — Identify the Premise

Before scoring, name the extraordinary condition at the heart of the narrative. State it in one sentence using plain language. If the premise cannot be stated without genre vocabulary (e.g. "a temporal anomaly causes..."), note this as the first sign of contamination.

The premise should be expressible as a simple human situation: "A man lives the same day repeatedly." "A woman wakes up as a different person each morning." "A family cannot leave their house."

### Step 2 — Score Each Dimension

Evaluate the submitted work against all ten dimensions (Zero through Nine) from the Essence of Groundhog. For each dimension, assign a score and provide specific evidence.

**Scoring Scale:**

| Score | Label | Meaning |
|-------|-------|---------|
| 5 | **Pure** | Full alignment. The dimension is honoured completely with no drift. |
| 4 | **Strong** | Mostly aligned. Minor moments of drift that could be corrected with light editing. |
| 3 | **Partial** | The intent is present but the execution introduces violations. Structural edits needed. |
| 2 | **Compromised** | Significant violations. The dimension is acknowledged but frequently undermined. |
| 1 | **Violated** | The work actively contradicts this dimension through its structure or content. |
| 0 | **Absent** | The dimension is not addressed at all — the work operates as though it does not exist. |

### Step 3 — Identify the Primary Violation Pattern

Most narratives that fail the Groundhog principles fail in a pattern, not randomly. Common patterns include:

- **Explanation Creep** — The narrative starts clean but gradually introduces explanatory scaffolding as if the writer lost confidence in the bare premise.
- **Guide Insertion** — A character who begins as ordinary slowly becomes a mentor or interpreter figure, often disguised as a love interest or friend.
- **Genre Drift** — The vocabulary, imagery, or tonal register slides toward science fiction, fantasy, or horror tropes without the writer appearing to notice.
- **Intellectual Arc Substitution** — The character's transformation is expressed through dialogue, internal monologue, or articulated realisations rather than accumulated behavioural change.
- **World Expansion Escape** — The narrative introduces new locations, characters, or rules to maintain interest rather than deepening what already exists.
- **Resolution Ceremony** — The ending features a marked, confirmed, or celebrated moment of release rather than a quiet, unmarked transition.
- **Tonal Collapse** — The work commits entirely to comedy or entirely to bleakness, losing the tension that makes the premise powerful.

Name the primary pattern and explain how it manifests in the specific work.

### Step 4 — Produce the Assessment Report

Output a markdown document following this structure:

```
# Groundhog Loop Assessment — [Title or Description of Work]

## Mode: [ASSESS / PLAN / WORLD]

## Premise (Plain Language)
[One sentence. No genre vocabulary.]

## Dimension Scores

| Dimension | Score | Label |
|-----------|-------|-------|
| D0 — Premise as Condition | X/5 | [Label] |
| D1 — No Guide | X/5 | [Label] |
| D2 — No Explanation | X/5 | [Label] |
| D3 — No Resolution Ceremony | X/5 | [Label] |
| D4 — No Science Fiction | X/5 | [Label] |
| D5 — Behavioural Arc | X/5 | [Label] |
| D6 — Small Fixed World | X/5 | [Label] |
| D7 — Real Characters | X/5 | [Label] |
| D8 — Comedy-Tragedy Tension | X/5 | [Label] |
| D9 — Premise Is Not the Point | X/5 | [Label] |
| **TOTAL** | **XX/50** | |

## Overall Alignment Grade

| Range | Grade | Meaning |
|-------|-------|---------|
| 45-50 | **FABLE** | The work operates as a pure moral fable. The premise is invisible. |
| 35-44 | **GROUNDED** | Strong human story with minor genre leakage. Correctable. |
| 25-34 | **MIXED** | The human story and the genre exercise are competing. Structural work needed. |
| 15-24 | **GENRE-BOUND** | The premise dominates. The character exists to serve the concept. |
| 0-14 | **MECHANISM** | The work is about its own premise. Fundamental reconception needed. |

Grade: [GRADE]

## Primary Violation Pattern
[Name and explain]

## Dimension Analysis
[For each dimension: 2-4 sentences explaining the score, citing specific moments, lines, characters, or structural choices from the submitted work. Be concrete — quote or reference specific passages.]

## Alignment Instructions
[Prioritised, actionable steps to move the work closer to full alignment. Number them. Start with the highest-impact changes. Each instruction should reference the specific dimension it addresses and explain not just what to change but why the current version violates the principle.]
```

### Step 5 — Present the Report

Save the assessment as `[title-or-identifier]-groundhog-assessment.md` in the output directory. If the input was a file, derive the name from the input filename.

---

## Guidance for Each Dimension

These notes help you apply the scoring consistently. Always cross-reference with the full grounding document for the definitive rules.

### D0 — Premise as Condition
The premise must function as weather the character lives inside, not a puzzle they investigate. If any character in the work spends meaningful time trying to understand, explain, or control the premise, the score drops. The premise is interesting to the audience only because of what it reveals about the character — never for its own sake.

### D1 — No Guide
Check every character who interacts with the protagonist. Does any of them function as an interpreter of the condition? This includes disguised guides: a love interest who "brings out the best" in the protagonist through wisdom rather than simply existing, a bartender who delivers thematic monologues, a child who says something impossibly insightful. The guide can be subtle — look for any character who seems to know more about the premise than the protagonist, even implicitly.

### D2 — No Explanation
Search for any causal framework. This includes: scientific causes, magical causes, religious causes, karmic causes, psychological causes ("it's happening because of your unresolved trauma"), and narrative causes ("the universe is trying to teach you"). Even implied explanation counts — if the audience could reasonably infer a cause from contextual clues the writer planted, the explanation exists.

### D3 — No Resolution Ceremony
Examine the ending. Is there a moment of triumph, confirmation, or acknowledgement? Does any character (including the protagonist) explicitly recognise that the condition has ended? Is the final scene emotionally pitched as a reward? The ideal ending is one where the audience feels something has changed but cannot point to the exact moment it happened.

### D4 — No Science Fiction
This is the vocabulary audit. Search the entire text for: temporal, quantum, paradox, loop, anomaly, glitch, rift, dimension, multiverse, simulation, matrix, code, program, algorithm, system, protocol, frequency, wavelength, radiation, energy field, portal, wormhole, singularity, timeline, alternate reality, parallel. Also search for any character who responds to the premise analytically rather than emotionally. A character who says "maybe if I do X differently the loop will break" is engaging in hypothesis-testing — that is scientific thinking applied to the premise, and it contaminates.

### D5 — Behavioural Arc
Map the protagonist's trajectory against the seven phases (Disorientation → Exploitation → Despair → Collapse → Quiet Turning → Accumulation → Unnoticed Arrival). Not every phase needs to be present, and they need not be sequential, but the overall shape should be behavioural rather than intellectual. The critical test: does the protagonist *articulate* their growth at any point? If they can explain what they've learned, the arc has been intellectualised.

### D6 — Small Fixed World
Count the locations, count the named characters, count the distinct events in the repeating period. Are new elements introduced after the first cycle? If yes, why? Expansion for its own sake (to avoid boring the audience) is a violation. Expansion that reveals hidden depth in what was already there (the protagonist finally notices a detail that was present all along) is alignment.

### D7 — Real Characters
For each named supporting character, ask: does this person have at least one detail that exists solely for them? Do they have an inner life the protagonist could discover but hasn't yet? Are they ever reduced to a function (obstacle, reward, comic relief, love interest) without remainder? The protagonist's growth is partly measured by their increasing perception of these people as full subjects.

### D8 — Comedy-Tragedy Tension
Read the work for tonal shifts. Is the same event or situation treated as both funny and devastating at different points (or simultaneously)? Does the work sustain a single register for too long? The ideal is a constant oscillation that prevents the audience from settling into comfort or despair.

### D9 — Premise Is Not the Point
The meta-test. If you had to describe this work in one sentence to someone who would never read it, would you mention the premise or the character? "It's about a man who relives the same day" is a genre description. "It's about a man who slowly learns to care about other people" is a human description. The work passes D9 when the second description is more accurate than the first.

---

## Handling Lorebooks and World Definitions (Mode 3)

When assessing a lorebook or world bible, the dimensions apply differently — you are evaluating whether the *world itself* is built to support or undermine the principles.

Key questions for world documents:

- Does the world contain a magic system, technology, or cosmology that would explain the premise? (D2 violation baked into the setting)
- Does the world contain a character archetype designated as a mentor, sage, or oracle? (D1 violation baked into the cast)
- Does the lore include terminology for the premise? (D4 violation baked into the vocabulary)
- Is the world large, expansive, and full of discoverable locations? (D6 tension — large worlds resist the confinement principle)
- Does the world's tone lean consistently comic, grimdark, or whimsical? (D8 tension — pre-committed tone)

For lorebooks, provide alignment instructions that restructure the world to *remove* explanatory architecture, *reduce* the cast to a confined ensemble, and *strip* genre vocabulary from the setting's own description of itself.

---

## Critical Reminders

- Always read `references/ESSENCE-of-GROUNDHOG.md` before assessing. Every time. The document is the authority, not your recollection of it.
- Be specific in your evidence. "This scene violates D4" is useless. "The line 'Maybe this is some kind of temporal anomaly' in Chapter 3 introduces science fiction vocabulary into a character's response to the premise" is useful.
- Alignment instructions must be prioritised by impact. The first instruction should address the violation that most damages the work's alignment overall.
- The skill is not hostile to the submitted work. It is a diagnostic tool. Frame all feedback as improvement toward a specific, well-defined standard — not as criticism of the writer's ability or intent.
- A low score is not failure — it is information. Many excellent genre stories would score 5/50 against these principles. The Groundhog standard is deliberately narrow and is designed for a specific kind of narrative. The skill should acknowledge this when appropriate.
