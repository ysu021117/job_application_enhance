---
name: job-application-strategy
description: Extract and normalize candidate experience from one or more resumes, CVs, portfolios, articles, transcripts, and related materials; then analyze a target job's responsibilities and requirements, compare them against the extracted evidence and available company information, and produce a targeted resume strategy before drafting final application documents. Use when Codex needs to consolidate multiple source versions into reusable reference files, evaluate job fit, recommend which content should appear in a resume, estimate application competitiveness, create a markdown resume blueprint, and then coordinate resume and optional cover-letter output with $career-voice-match.
---

# Job Application Strategy

## Overview

Use this skill to decide what a candidate has actually done, what matters for a target role, and what should be highlighted before any polished drafting begins. Separate evidence extraction, job-fit analysis, and final document generation into distinct stages.

## Skill Structure

Keep two layers separate:

- `references/`: static, skill-owned method documents
- workspace: dynamic task artifacts created in the parent folder of this skill

On first use, create a sibling workspace such as `../job-application-strategy-workspace/`.

Use this workspace structure:

- `source/`: user-provided resumes, portfolios, transcripts, job descriptions, and company notes
- `reference/`: extracted candidate evidence and normalized experience records
- `analysis/`: job-fit analysis, success estimate, and resume-content recommendations
- `output/`: markdown blueprint and final document outputs

Use the templates in `assets/templates/` to create dynamic files in the workspace. Do not place user-derived data inside `references/`.

## Inputs

Expect some or all of the following:

- one or more resume or CV versions
- supporting materials such as portfolio pieces, articles, transcripts, bios, project lists, or past application documents
- a target job description
- optional company information, hiring context, or user priorities
- optional reference resume or cover-letter document whose formatting should be preserved in the final Word output
- optional instruction about whether to produce only a resume or also prepare for a cover letter

## Core Goal

Produce a hiring-targeted strategy that:

- extracts what the user has actually done across multiple source versions
- preserves quantified evidence completely
- identifies the most important responsibilities and requirements in the target role
- estimates how competitive the application is using explicit reasoning rather than guesswork
- recommends what content should be emphasized in the resume
- generates a markdown resume blueprint before final document drafting

## Operating Principles

- Extract facts, not polished source wording.
- Preserve quantified content even when wording varies across source files.
- Reconcile multiple versions into normalized evidence records.
- Base fit analysis on the target role, the company context, and the extracted reference set.
- Treat the success estimate as a heuristic assessment, not a prediction.
- Tie every success estimate to explicit evidence dimensions rather than general impression.
- When a reference document is supplied for final output, preserve its layout system in the final Word file, including heading treatment, font choices, spacing, and page-length constraints.
- Do not draft final resume or cover letter wording until the user approves the markdown blueprint.

## Workflow

1. On first use, create the workspace with `source/`, `reference/`, `analysis/`, and `output/`.
2. Collect the user's source materials and target job information in `source/`.
3. Extract and normalize candidate experience into reusable reference files in `reference/`.
4. Read the job description and company context, then identify the highest-priority responsibilities and requirements.
5. Compare the job priorities against the extracted reference set and produce an analysis with:
   - key matches
   - notable gaps
   - estimated application success range with reasoning
   - recommendations for what to foreground in the resume
6. Create a markdown resume blueprint in `output/` that reflects the recommended content selection and structure.
7. Present the analysis and blueprint to the user and wait for approval or corrections.
8. After approval, use the blueprint plus `$career-voice-match` to produce a resume Word document.
9. Only produce a cover-letter Word document if the user asks for it after reviewing the resume plan or final resume.

Use these references as needed:

- [references/workspace-setup.md](references/workspace-setup.md)
- [references/source-extraction.md](references/source-extraction.md)
- [references/job-fit-analysis.md](references/job-fit-analysis.md)
- [references/output-pipeline.md](references/output-pipeline.md)
- [references/word-format-fidelity.md](references/word-format-fidelity.md)

## Outputs

Default outputs are:

- `reference/master-experience-reference.md`
- `analysis/job-fit-analysis.md`
- `output/resume-blueprint.md`

After user approval, additional outputs can include:

- `output/resume.docx`
- `output/cover-letter.docx`

## Style Rules

- Keep extraction files factual and compressed.
- Keep analysis reasoning concrete and evidence-based.
- Do not hide meaningful gaps between the candidate and the role.
- Make recommendations specific enough that a final resume can be drafted from the blueprint.

## Example Triggers

Use this skill for requests like:

- "Combine these resume versions and tell me what to emphasize for this job."
- "Read my transcript and portfolio, then decide whether I should apply to this role."
- "Extract my strongest evidence and create a targeted resume plan for this posting."
- "Tell me my chances for this role and draft the best resume direction before we write it."
