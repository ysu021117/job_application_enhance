# Output Pipeline

Use this reference after extraction and analysis are complete.

## Goal

Convert the analysis into a user-reviewable markdown blueprint first, then produce final application documents only after approval.

## Required Order

Follow this order:

1. build the extracted reference set
2. complete the job-fit analysis
3. create `output/resume-blueprint.md`
4. wait for user approval or corrections
5. produce `output/resume.docx`
6. optionally produce `output/cover-letter.docx` if the user asks

## Resume Blueprint

The markdown blueprint should include:

- target role and company
- proposed headline or summary direction
- which experiences to foreground
- which quantified achievements to include
- which skills or subject areas to highlight
- section-level content guidance
- optional notes on what to omit or compress

The blueprint is not the final polished resume. It is the content plan.

Start from `assets/templates/resume-blueprint-template.md` when useful.

## Final Drafting Handoff

After the user approves the blueprint:

- use the approved blueprint as the content source of truth
- use `$career-voice-match` to align the writing style with the user's voice
- produce the resume as a Word document
- if a reference resume document is provided, preserve its formatting system exactly in the Word output

If the user wants a cover letter:

- derive it from the approved blueprint, job analysis, and company context
- use `$career-voice-match` for tone alignment
- output it as a Word document after the resume or alongside it if the user explicitly asks
- if a reference cover-letter document is provided, preserve its formatting system exactly in the Word output

## Document Output

Prefer `.docx` output for final deliverables when the environment supports document generation. If `.docx` generation is not available in the current environment, state that clearly and return the best available markdown draft instead.

When a reference document is supplied for formatting:

- preserve font family, font sizing pattern, line spacing, paragraph spacing, margins, section spacing, and heading treatment
- preserve the overall visual hierarchy, including how headings, subheadings, and section labels are styled
- preserve page-length constraints
- if the reference resume is one page, the final rewritten resume must also remain one page
- if keeping the content within the same page count requires compression, tighten wording and content selection rather than allowing overflow by default
