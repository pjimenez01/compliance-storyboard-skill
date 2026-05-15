---
name: compliance-storyboard
description: A compliance training storyboard generator grounded in strong instructional design principles, adaptable to any organisation or regulatory context. Use this skill whenever a user provides compliance content — such as a policy document, regulatory outline, or draft training material — and wants it converted into a structured storyboard ready for eLearning development. Trigger when users mention "storyboard", "compliance training", "eLearning module", "course outline", "training script", or ask to turn a policy, regulation, or compliance document into a training course. Also use when a compliance professional wants help writing learning objectives, narration scripts, knowledge checks, or interactive scenarios from source compliance content.
---

# Compliance Training Storyboard Skill

This skill transforms raw compliance content into a complete, instructionally sound storyboard for eLearning development. It is designed for use by compliance subject matter experts (SMEs) who are knowledgeable in regulations but not trained in instructional design.

The output is a downloadable `.docx` file structured as a storyboard that an SME can review and edit, then hand off to a learning designer for development.

---

## Who This Is For

**Primary users:** Compliance subject matter experts (SMEs) who are knowledgeable in regulations but not trained in instructional design.
**Their input:** Draft compliance content — most commonly a structured document or slide deck (e.g., Google Docs or Google Slides) — that is accurate but not yet designed for learning. Other formats are supported.
**Their output:** A complete storyboard they can review, refine, and hand off to a learning designer for development.

---

## Core Design Principles

Every storyboard must reflect these four principles:

1. **User-Centricity** — Content is clear, intuitive, and easy to navigate. Learners can quickly understand what they need to know and do. Avoid jargon where possible and prioritise helping the learner take action.
2. **Engaging Storytelling** — Training reads as a cohesive, purposeful narrative — not a list of rules. Provide context, highlight why the content matters, and drive action. The "why" should always be visible.
3. **On-Brand Relevance** — Examples and scenarios should feel aligned to the organisation, its products, and its compliance priorities. When possible, situations should reflect realistic, role-relevant workplace contexts drawn directly from the source content.
4. **Evolving with Agility** — Structure should be modular and easy to update. Each section should be independently revisable as regulations, policies, or priorities change over time.

---

## Compliance Constraints

These are non-negotiable:

- **Do not rewrite or reinterpret regulations.** Regulatory language must remain accurate and intact. You may clarify or explain concepts in plain language, but never alter the meaning or intent of the original content.
- **Maximum course length is 1 hour.** Scope the storyboard accordingly. Prioritise the most critical content and organise efficiently.
- **Scenarios and examples must be grounded in the source material.** Do not invent situations that go beyond what the source content covers.
- **Maximum 3 scenarios per course.** Place them strategically at points where application of a concept is most valuable.

---

## Document Formatting Standards

Apply these standards to every storyboard output without exception:

- **Font:** Montserrat throughout — headings, body text, labels, captions, and table content.
- **Text colour:** Pure black (`#000000`) for all text.
- **Primary brand colour:** Black (`#000000`) for all header bars, section banners, and table headers.
- **White text** on black backgrounds only.
- **Accent colours** permitted for feedback states only: green for correct feedback, red/light red for incorrect feedback, amber for callout/warning boxes.

When generating the `.docx` output, use the `docx` skill. Read `/mnt/skills/public/docx/SKILL.md` before writing any document code.

---

## Step 1: Analyse the Source Content

Before writing anything, read and analyse the input carefully. Identify:

- The core compliance topic and regulatory context
- The key rules, expectations, or obligations the learner must understand
- Any existing examples or scenarios in the source material
- Gaps in instructional structure (missing objectives, no narrative flow, no interactivity, etc.)
- The intended audience and any localisation needs (e.g., UK/Australian English)

If the input does not specify an audience, assume a broad employee population across multiple departments.

---

## Step 2: Write Learning Objectives

Write **3–5 learning objectives** using Bloom's Taxonomy, levels 1–4 only (Remember, Understand, Apply, Analyse).

Rules:
- Begin each with a measurable action verb
- Frame from the learner's perspective: "By the end of this course, you will be able to…"
- Align directly to the compliance content — do not introduce concepts not in the source
- Keep language clear and jargon-free

**Bloom's Level Reference (levels 1–4 only):**

| Level | Verbs to Use |
|---|---|
| 1 – Remember | identify, recall, list, name, define |
| 2 – Understand | explain, describe, summarise, classify |
| 3 – Apply | apply, use, demonstrate, solve, complete |
| 4 – Analyse | distinguish, compare, differentiate, examine |

---

## Step 3: Design the Course Structure

Organise the content into a logical, learner-friendly flow. Do **not** mirror the structure of the source document — redesign it for comprehension and progression.

### Recommended Module Arc

Adapt this structure based on content volume. Target total length: **30–60 minutes**.

```
1. Course Introduction
   - Video hook: why this matters to the learner (narrated)
   - [Learning objectives appear in Course Overview, not as a lesson screen]

2. Section 1: Context & Foundations
   - Why this regulation or policy exists
   - Who it applies to and why it matters in their role

3. Section 2–N: Core Concepts (one section per major topic area)
   - Explain the rule or requirement in plain language
   - Clarify regulatory language without altering its meaning
   - Specific visual suggestion for each screen
   - Scenario at the most appropriate section (max 3 total)
   - Mid-section knowledge check (1–2 questions) where appropriate

4. Summary & Key Takeaways
   - Recap of core concepts
   - Resource links and next steps

5. Cumulative Knowledge Check
   - 5–10 questions covering all learning objectives
```

### Timing Guidelines

| Element | Estimated Time |
|---|---|
| Introduction (video) | 2–3 minutes |
| Each core concept section | 5–8 minutes |
| Each scenario | 2–4 minutes |
| Each knowledge check question | ~30 seconds |
| Summary | 2–3 minutes |

---

## Step 4: Write the Storyboard

### Learning Objectives Placement

Learning objectives belong in the **Course Overview section of the document**, not as a lesson screen in the storyboard flow. Do not create a dedicated "Learning Objectives" lesson card (e.g., "Intro.2"). Present them as a numbered list under the Course Overview heading.

### Narration Rules

**Narration scripts are only included for video screens and scenario screens.**

- **Video screens** (typically the course introduction/hook): include a full narration script.
- **Scenario screens**: include narration for both the correct and incorrect outcome paths.
- **All other screen types** (Concept, Summary, Resource, Knowledge Check): do **not** include a narration field. These are static screens the learner reads independently.

### Visual Suggestion Rules

Every screen must include a Visual Suggestion. Visual suggestions must be **specific and actionable** — detailed enough for a designer to brief an illustrator or build the screen without further clarification.

Each Visual Suggestion must specify:
- **Format** (e.g., static infographic, two-column comparison table, horizontal process flow, decision tree, hub-and-spoke diagram, illustrated split-screen)
- **Layout** (number of columns, rows, panels, steps, nodes)
- **Content of each element** (what each icon, label, column, or row depicts — drawn from the source material)
- **Colour guidance** (which elements use which background or accent colours)
- **Typography** (approximate font sizes for labels vs. body text where helpful)

Vague suggestions like "use an infographic" or "show a diagram" are not acceptable. Be specific about what the visual depicts.

---

### Standard Screen Template

```
[Section N.Lesson N] — [Lesson Title]
Screen Type: [Video | Concept | Scenario | Knowledge Check | Summary | Resource]

ON-SCREEN TEXT
Headline: [1–2 line headline the learner sees on screen]
Body Text: [Supporting bullet points or short paragraph. No more than 3–4 bullets or 2–3 sentences.]

NARRATION SCRIPT
[Include ONLY for Video and Scenario screens. For all other screen types, omit this field entirely.]

VISUAL SUGGESTION
[Specific, actionable visual brief. See Visual Suggestion Rules above.]

INTERACTIVITY NOTE (if applicable)
[Flag if this screen should be interactive. One sentence, practical. Only include where genuinely useful.]

DESIGN NOTE (if applicable)
[One plain-language sentence explaining why this element was included. Only include where helpful to the SME. Omit if obvious.]
```

---

### Knowledge Check Template

```
[Section N.Lesson N] — Knowledge Check
Screen Type: Knowledge Check

QUESTION [N]:
[Question text — clear, direct, tied to source content]

A) [Option]
B) [Option]
C) [Option]
D) [Option]

Correct Answer: [Letter]
Feedback (correct): [1–2 sentences reinforcing why this is right]
Feedback (incorrect): [1–2 sentences redirecting the learner. Do not simply restate the question.]
```

---

### Scenario / Decision Point Template

```
[Section N.Lesson N] — Scenario: [Short Title]
Screen Type: Scenario
[Label as: Scenario X of 3 · Section N]

SETUP
[2–3 sentences. Realistic workplace situation drawn from source content. Name the character(s), give them a role, place them in context.]

DECISION PROMPT
[What should [character name] do?]

OPTION A: [Action]
→ Outcome: [What happens and why this is or isn't correct.]

OPTION B: [Action]
→ Outcome: [What happens and why this is or isn't correct.]

OPTION C: [Action]
→ Outcome: [What happens and why this is or isn't correct.]

CORRECT CHOICE: [Letter]

NARRATION (correct path): [Script reinforcing the right choice — firm, encouraging, not patronising.]
NARRATION (incorrect path): [Script redirecting — clear about what went wrong, not shaming.]

VISUAL SUGGESTION
[Illustrated split-screen layout. Left panel (60%): scene with named character(s), setting details, and a visible cue for the decision moment (e.g., speech bubble, screen content, expression). Right panel (40%): three stacked option buttons A/B/C — correct highlights green on selection, incorrect highlights red. Include screen label top-left: 'Scenario X of 3 · Section N.']

DESIGN NOTE (if applicable)
[One sentence. Only if helpful to the SME.]
```

---

## Step 5: Write the Cumulative Knowledge Check

At the end of the course, include a **5–10 question cumulative assessment** covering all learning objectives.

Rules:
- At least one question per learning objective
- Mix conceptual questions (understanding the rule) with application questions (what would you do)
- All questions must be traceable to the source content
- Use the Knowledge Check Template above for each question
- Include a passing score recommendation (80% or above)

---

## Step 6: Format the Full Document

Structure the complete storyboard document in this order:

```
COVER
  Course Title
  Target Audience
  Compliance Domain
  Estimated Duration
  Version / Date
  Prepared by: [SME name]

COURSE OVERVIEW
  Purpose Statement (1–2 sentences)
  Learning Objectives (numbered list — placed here, not in lesson flow)
  Course Structure Overview (section titles + types + estimated times)

STORYBOARD CONTENT
  [All sections and lessons using templates above]
  [Max 3 scenario screens, labelled Scenario 1/2/3 of 3]

CUMULATIVE KNOWLEDGE CHECK

APPENDIX (optional)
  Glossary of key terms (defined on first use in the storyboard)
  Regulatory references
  Key resources and links
```

---

## Tone and Language Standards

- **Clarity first.** Write for a broad employee audience, not specialists.
- **Professional but human.** Avoid stiff, legalistic phrasing. Regulatory text may be quoted accurately but must be followed by a plain-language explanation.
- **Active voice.** "You must report within 30 days" — not "Reports are required to be submitted within 30 days."
- **Localisation.** If the audience is in the UK, Australia, or another non-US market, apply local English conventions consistently (e.g., "organisation," "recognise," "licence"). Default to the conventions of the source material.
- **Jargon.** Define compliance terms and regulatory acronyms on first use. Include defined terms in the Appendix glossary.

---

## Instructional Design Principles (Applied, Not Named)

Apply these frameworks in how the storyboard is structured and written. Do **not** reference them by name in the output — just apply them:

- **Knowles' Andragogy:** Make content feel relevant to the learner's actual job. Always connect rules to real responsibilities.
- **Gagné's Nine Events:** Structure each section to gain attention, present the objective, activate prior knowledge, deliver content, provide examples, prompt practice, give feedback, assess, and reinforce retention.
- **Merrill's Principles:** Anchor content in real-world problems. Demonstrate before asking learners to apply. Connect new knowledge to existing understanding.
- **Bloom's Taxonomy (levels 1–4):** Sequence learning from recall → understanding → application → analysis. Ground concepts before asking learners to apply them.

---

## Quality Checklist

Before delivering the storyboard, verify:

- [ ] All learning objectives are covered by at least one lesson or scenario
- [ ] Learning objectives appear in the Course Overview — not as a lesson screen
- [ ] Regulatory language is accurate and unaltered throughout
- [ ] All scenarios are grounded in the source content — nothing invented
- [ ] Narration included only on Video and Scenario screens — omitted from all others
- [ ] Every screen has a specific, actionable Visual Suggestion
- [ ] No more than 3 scenarios in the course — each labelled "Scenario X of 3"
- [ ] Knowledge check questions are tied directly to source content
- [ ] Cumulative assessment covers all objectives with a passing score noted
- [ ] Estimated total duration is within 1 hour
- [ ] Document uses Montserrat font and black (#000000) text throughout
- [ ] Localisation applied correctly if specified
- [ ] Core design principles (user-centricity, engaging storytelling, on-brand relevance, agility) are evident throughout
- [ ] Design notes are brief, plain-language, and minimal — omitted where obvious
