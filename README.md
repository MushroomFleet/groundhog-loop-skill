# Groundhog Loop

A Claude skill for assessing and aligning narrative works with the **Essence of Groundhog** principles — a behavioural ruleset for stories that use extraordinary premises to explore ordinary human transformation, without any reliance on science fiction, guides, explanations, or marked resolutions.

Derived from the structural architecture of *Groundhog Day* (1993, Ramis/Rubin), this skill treats the film not as a plot to be imitated but as a set of narrative principles to be followed. The core insight: *Groundhog Day* is arguably the only time loop film to achieve universal cultural significance precisely because it escaped the trappings of science fiction entirely. There is no guide, no explanation, and no resolution — the condition simply begins, the character changes through behaviour rather than understanding, and one morning it ends without ceremony.

This skill captures those principles as a diagnostic and alignment tool for any narrative built around an extraordinary premise.

---

## The Grounding Artifact

At the heart of this skill is **ESSENCE-of-GROUNDHOG.md**, a grounding document that codifies ten dimensions of narrative architecture:

| Dimension | Principle |
|-----------|-----------|
| **D0** — Prime Directive | The premise is the condition, never the subject |
| **D1** — No Guide | No mentor, teacher, or interpreter of the condition |
| **D2** — No Explanation | No origin, cause, mythology, or explanatory scaffolding |
| **D3** — No Resolution | No confirmation, ceremony, or acknowledgement of release |
| **D4** — No Science Fiction | Zero genre vocabulary, technology, or analytical framing |
| **D5** — Behavioural Arc | Transformation through accumulated action, not revelation |
| **D6** — Small Fixed World | Confinement that demands depth over breadth |
| **D7** — Real Characters | Supporting cast with independent inner lives |
| **D8** — Comedy-Tragedy Tension | Tonal ambiguity sustained throughout |
| **D9** — Premise Is Not the Point | The human question is the only question |

Each dimension includes specific generation rules and vocabulary-level audit criteria. The full document is bundled with the skill at `references/ESSENCE-of-GROUNDHOG.md`.

---

## Three Modes of Operation

### Mode 1 — ASSESS
Submit finished or draft **prose, screenplay pages, or chapters**. The skill scores alignment with each dimension, identifies specific violations with cited evidence, and provides prioritised correction instructions.

### Mode 2 — PLAN
Submit a **story outline, beat sheet, synopsis, or plot summary**. The skill evaluates structural alignment and flags where the plan is likely to produce violations when written — catching problems before they're embedded in prose.

### Mode 3 — WORLD
Submit a **lorebook.md, world bible, setting document, or character roster**. The skill assesses whether the world architecture itself supports or undermines the principles — particularly whether built-in explanation systems, guide archetypes, or genre scaffolding would contaminate any narrative set within it.

---

## Scoring

Each dimension is scored 0–5:

| Score | Label | Meaning |
|-------|-------|---------|
| 5 | Pure | Full alignment, no drift |
| 4 | Strong | Mostly aligned, light edits needed |
| 3 | Partial | Intent present, execution introduces violations |
| 2 | Compromised | Significant violations undermine the dimension |
| 1 | Violated | The work actively contradicts this dimension |
| 0 | Absent | The dimension is not addressed at all |

Total scores map to an overall alignment grade:

| Range | Grade | Meaning |
|-------|-------|---------|
| 45–50 | **FABLE** | Pure moral fable. The premise is invisible. |
| 35–44 | **GROUNDED** | Strong human story with minor genre leakage. |
| 25–34 | **MIXED** | Human story and genre exercise are competing. |
| 15–24 | **GENRE-BOUND** | The premise dominates the character. |
| 0–14 | **MECHANISM** | The work is about its own premise. |

A low score is not failure — it is information. Many excellent genre stories would score near zero against these principles. The Groundhog standard is deliberately narrow, designed for a specific kind of narrative where the human question is the only question that matters.

---

## Violation Patterns

The skill identifies common failure patterns by name:

- **Explanation Creep** — Gradual introduction of explanatory scaffolding as the writer loses confidence in the bare premise
- **Guide Insertion** — A character who begins as ordinary slowly becomes a mentor, often disguised as a love interest
- **Genre Drift** — Vocabulary, imagery, or tonal register slides toward science fiction tropes without the writer noticing
- **Intellectual Arc Substitution** — Transformation expressed through dialogue or internal monologue rather than behavioural change
- **World Expansion Escape** — New locations and characters introduced to maintain interest rather than deepening what exists
- **Resolution Ceremony** — The ending features a marked, celebrated moment of release rather than a quiet transition
- **Tonal Collapse** — The work commits entirely to comedy or bleakness, losing the tension

---

## Installation

Download the `groundhog-loop.skill` file from [Releases](https://github.com/MushroomFleet/groundhog-loop-skill/releases) and install it in your Claude skill directory.

The skill contains:
```
groundhog-loop/
├── SKILL.md                              # Assessment engine and instructions
└── references/
    └── ESSENCE-of-GROUNDHOG.md           # Grounding artifact (authoritative source)
```

---

## Usage

Trigger the skill by submitting any narrative work alongside a request for assessment:

> "Assess my story outline against groundhog principles"

> "Is my loop narrative too sci-fi? Here's the first three chapters..."

> "Check this lorebook for genre contamination"

> "Groundhog-loop assessment of my screenplay"

The skill reads the grounding artifact fresh before every assessment, scores all ten dimensions with specific evidence from the submitted work, and outputs a structured markdown report with prioritised alignment instructions.

---

## The Argument Behind the Skill

*Groundhog Day* stands alone among time loop films because it escaped the genre entirely. There is no machine, no scientist, no third-act revelation about why February 2nd keeps repeating. The loop is not a puzzle — it is weather. Phil Connors is not solving anything. He is simply a man trapped inside a condition, and the film watches what he does with it.

No guide curates the experience. No explanation gives it meaning. No resolution confirms he passed. He goes through selfishness, hedonism, despair, and attempted suicide — and then, without announcement, begins doing small things differently. The transformation is behavioural, not intellectual. He never articulates what he learned. He just becomes someone different, and one morning it's February 3rd, and the film doesn't explain that either.

That structural choice — no guide, no explanation, no resolution — is why the film sits next to *It's a Wonderful Life* rather than next to *Looper*. It belongs to the tradition of moral fables, not science fiction. And it is why "Groundhog Day" entered the language itself as a phrase meaning something far deeper than its plot.

This skill exists to help writers build stories that operate in the same tradition: extraordinary premises used as pure vehicles for the ordinary, difficult, accumulative work of human transformation.

---

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{groundhog_loop_skill,
  title = {Groundhog Loop Skill: Narrative Assessment Against Essence of Groundhog Principles},
  author = {Drift Johnson},
  year = {2025},
  url = {https://github.com/MushroomFleet/groundhog-loop-skill},
  version = {1.0.0}
}
```

### Donate:

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)
