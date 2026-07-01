# Reference Management

Use this reference when the user provides prior writing and wants that material to guide future resume or cover-letter edits.

## Goal

Convert past writing into a reusable voice reference without treating the past writing as a source of facts for the new document.

## Ownership Boundary

Separate reference material into two classes:

- static references: method documents bundled with the skill
- dynamic references: user-derived voice artifacts created in the workspace during use

Static references explain how to analyze tone.
Dynamic references capture what was learned about one user's tone.

Do not overwrite static references with user-specific findings.

## Reading Order

Read provided materials in this order:

1. target resume or cover letter
2. explicit optimization request
3. past professional writing samples
4. any user notes about tone preferences

This order prevents sample tone from overriding the factual boundaries of the target document.

## How To Read Past Writing

Read samples in three layers:

### Layer 1: audience and context

Identify what kind of document each sample is:

- internal email
- client-facing email
- statement of purpose
- networking note
- performance self-review
- previous cover letter

This helps decide how transferable the tone is.

### Layer 2: stable voice traits

Extract traits that are likely to carry across contexts:

- concise or expansive
- plainspoken or elevated
- warm or reserved
- direct or diplomatic
- modest or assertive
- smooth and polished or brisk and practical

These traits are valid reference material.

### Layer 3: non-transferable material

Mark content that should not be carried forward as voice guidance:

- role-specific facts
- company names
- confidential information
- one-off emotional language
- temporary urgency
- content written for a very different audience

Do not let these distort the rewrite.

## How To Build A Reusable Reference

When enough sample material exists, convert it into a compact artifact such as `dynamic-reference/voice-reference.md`.

Recommended structure:

1. one-line voice summary
2. tone sliders
3. preferred moves
4. avoid list
5. resume-specific guardrails
6. cover-letter-specific guardrails

Example:

- Voice summary: "Measured, direct, and polished. Prefers clarity over flourish."
- Tone sliders: medium formality, high clarity, moderate warmth, low hype
- Preferred moves: short openings, concrete verbs, no dramatic claims
- Avoid list: "passionate," "dynamic," overly ceremonial transitions

Start from the template at `assets/templates/voice-reference-template.md` when available.

## Rules For Ongoing Reuse

When a saved voice reference exists in the workspace:

- use it as a style prior, not a factual source
- update it only when new samples show a stable pattern
- prefer explicit user corrections over older inferred patterns
- keep it compact so it stays readable and reusable

If new samples conflict with the saved reference:

1. trust explicit user instruction first
2. trust newer professional samples second
3. update only the traits that clearly changed

## Storage Rules

Use `references/` only for static skill-owned guidance.

Use the workspace `dynamic-reference/` folder for dynamic user-derived files such as:

- `voice-reference.md`
- `preferred-phrasing.md`
- `avoid-patterns.md`
- `application-tone-notes.md`

If only one dynamic file is needed, prefer a single compact `voice-reference.md`.

If raw user writing must be retained for traceability, keep it separate from the summarized reference and label it clearly as source material rather than reusable guidance.

## Privacy And Compression

Prefer summarizing samples over storing them verbatim.

Good reference material:

- "Prefers direct openings"
- "Avoids inflated adjectives"
- "Usually sounds warm but concise"

Poor reference material:

- full copied emails
- sensitive names or private details
- long excerpts that encourage imitation instead of pattern matching
