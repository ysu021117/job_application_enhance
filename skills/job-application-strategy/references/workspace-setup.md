# Workspace Setup

Use this reference on the first run of the skill or whenever no active workspace exists.

## Goal

Create a dedicated work area outside the static skill package so source files, extracted references, analysis artifacts, and final outputs stay separate from the skill itself.

## Workspace Location

Create the workspace in the parent folder of the skill.

Recommended name:

- `job-application-strategy-workspace`

Recommended structure:

- `job-application-strategy-workspace/source/`
- `job-application-strategy-workspace/reference/`
- `job-application-strategy-workspace/analysis/`
- `job-application-strategy-workspace/output/`

## Folder Purposes

- `source/`: original resumes, portfolio materials, transcripts, job descriptions, and company notes
- `reference/`: normalized candidate evidence extracted from the source materials
- `analysis/`: job-fit analysis and content-selection decisions
- `output/`: markdown blueprint and final document outputs

## First-Use Interaction Flow

Follow this sequence:

1. create the workspace folders
2. ask the user to provide source resumes and any additional evidence files
3. ask for the target job description and any company notes
4. explain that you will first extract evidence, then produce a strategy and markdown blueprint
5. deliver the analysis and blueprint
6. wait for user approval before producing the final resume document

Do not start final drafting immediately unless the user explicitly asks to skip the checkpoint.
