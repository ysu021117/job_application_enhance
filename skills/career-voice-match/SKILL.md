---
name: career-voice-match
description: Revise English resumes and cover letters so they sound more natural, professional, and aligned with the user's real writing voice. Use when Codex needs to improve or rewrite a resume, CV, cover letter, job application draft, LinkedIn summary, or other career-facing document while preserving the user's facts and matching tone from supplied professional writing samples, tone notes, or style preferences.
---

# Career Voice Match

## Overview

Use this skill to make career documents sound like a thoughtful person wrote them, not a generic assistant. Keep the writing credible, concise, and professional while adapting it to the user's natural English voice.

## Skill Structure

Keep two layers separate:

- `references/`: static, skill-owned method documents inside the skill package
- workspace: dynamic, user-derived files created in the parent folder of this skill

On first use, create a sibling workspace next to the skill folder, such as `../career-voice-match-workspace/`.

Use this workspace structure:

- `input/`: target resume, cover letter, and user requirement notes
- `dynamic-reference/`: user-derived voice artifacts and source writing samples
- `output/`: revised documents

Use `assets/templates/voice-reference-template.md` as the starting point for reusable user-specific references. Do not store user-derived tone notes inside `references/`.

## Inputs

Expect some or all of the following:

- A resume, CV, cover letter, or job-application draft
- A request such as "make this sound more natural," "less stiff," "more confident," or "closer to how I write"
- Optional professional writing samples such as emails, statements, outreach notes, summaries, or prior application materials
- Optional reference document whose layout and Word formatting should be preserved
- Optional context such as target role, company, industry, seniority, or tone constraints

Treat professional writing samples as the highest-value source for voice calibration. If samples are missing, rely on the user's explicit preferences and the document's existing tone.

## Core Goal

Produce a stronger English resume or cover letter that:

- sounds natural and human
- preserves all factual content unless the user asks for substantive edits
- reflects the user's own professional voice rather than a generic polished template
- stays appropriate for hiring contexts

## Operating Principles

- Preserve facts and claim strength.
- Improve language, not biography.
- Match stable voice patterns, not exact phrasing.
- Prefer the smallest rewrite that solves the user's request.
- Treat user samples as tone evidence, not content to copy.
- Verify that the final draft is consistent with the user's supplied references before delivering it.
- When revising a Word document against a reference layout, preserve the reference document's formatting system and page-length constraints.

For detailed preservation boundaries and editable surface area, read [references/editing-boundaries.md](references/editing-boundaries.md).

## Workflow

1. On first use, create a workspace in the parent folder of this skill with `input/`, `dynamic-reference/`, and `output/`.
2. Confirm what file needs revision and what direction the user wants, then save the working materials in `input/`.
3. Ask the user to provide past professional writing samples if no adequate reusable voice reference already exists.
4. Review the target document first for facts, then for style issues. Review user samples for stable voice signals only.
5. Present a short modification plan and wait for user confirmation or added requirements.
6. After user approval, rewrite with genre-appropriate constraints.
7. Run a final consistency check against the user's writing samples or saved voice reference. If the draft does not sound aligned, revise again before delivery.
8. If a formatting reference document exists, run a final format-fidelity check for layout, headings, spacing, font pattern, and page count.
9. Save the result in `output/`. When reuse is likely, create or update a compact dynamic `dynamic-reference/voice-reference.md`.

Use these references as needed:

- [references/editing-boundaries.md](references/editing-boundaries.md)
- [references/voice-calibration.md](references/voice-calibration.md)
- [references/reference-consistency-check.md](references/reference-consistency-check.md)
- [references/reference-management.md](references/reference-management.md)
- [references/workspace-setup.md](references/workspace-setup.md)
- [references/kickoff-protocol.md](references/kickoff-protocol.md)
- [references/word-format-fidelity.md](references/word-format-fidelity.md)

## Output

Default to saving the revised document in `output/` and returning the result to the user.

If helpful and brief, add 2 to 4 short notes after the rewrite covering major tone choices, but only when the user asks for explanation or when a tradeoff materially affects the result.

## Style Rules

- Write in English unless the user asks otherwise.
- Sound polished, not robotic.
- Avoid generic corporate filler and obvious AI phrasing.
- Do not add unsupported claims or closely copy sample wording.

## Example Triggers

Use this skill for requests like:

- "Rewrite my resume so it sounds more like me."
- "Make this cover letter less AI-ish."
- "Use my past emails to match my tone in this job application."
- "Polish this CV, but keep my voice and don't make it too formal."
