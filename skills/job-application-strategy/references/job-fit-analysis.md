# Job Fit Analysis

Use this reference when turning the extracted candidate reference set into a targeted application strategy.

## Goal

Identify what matters most in the target role, compare it against the candidate's evidence, and recommend how to position the application.

## Inputs

Read:

- the target job description
- any supplied company information
- the extracted candidate reference files

## Analysis Tasks

1. extract the highest-priority responsibilities
2. extract the highest-priority requirements and preference signals
3. identify the strongest evidence matches in the candidate reference
4. identify meaningful gaps or weakly supported areas
5. determine which experiences should be foregrounded in the resume

## Priority Signals

Give extra weight to:

- repeated requirements
- requirements near the top of the posting
- responsibilities tied to core ownership
- domain-specific experience that is central to the company or role
- evidence that clearly separates required from preferred qualifications

## Success Estimate

Provide an estimated application-success band using explicit reasoning.

Use a simple band such as:

- strong
- moderate
- stretch
- weak

Explain the estimate with evidence. Do not present it as a prediction or certainty.

Base the estimate on these dimensions:

- required qualification coverage
- strength of direct experience match
- quality and quantity of quantified evidence
- domain or industry alignment
- seniority alignment
- presence of critical gaps

## Band Guidance

Use the bands consistently:

- `strong`: the candidate covers most critical requirements, has several direct evidence matches, and has no major unaddressed gap in the core role
- `moderate`: the candidate covers many important requirements, but some higher-priority items are weaker, indirect, or less proven
- `stretch`: the candidate has some relevant signals, but important requirements or core ownership areas are thin, indirect, or missing
- `weak`: the candidate lacks multiple central requirements or the available evidence is too limited to support a competitive application

## How To Explain The Estimate

Do not only name the band. Explain:

1. which requirements are strongly supported
2. which important requirements are only partially supported
3. which gaps materially reduce competitiveness
4. whether a tailored resume can improve positioning or only clarify existing strengths

When the fit is borderline, say so clearly. Avoid overconfident encouragement.

## Required Analysis Output

Create `analysis/job-fit-analysis.md` with:

- role summary
- top responsibilities
- top requirements
- strongest evidence matches
- notable gaps
- success estimate with reasoning
- recommended resume emphasis
- content to deprioritize or omit

Start from `assets/templates/job-fit-analysis-template.md` when useful.
