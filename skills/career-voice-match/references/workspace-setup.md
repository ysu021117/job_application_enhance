# Workspace Setup

Use this reference on the first run of the skill or whenever no active workspace exists yet.

## Goal

Create a dedicated working area outside the static skill package so user-derived files, source materials, and outputs stay separate from the skill itself.

## Workspace Location

Create the workspace in the parent folder of the skill.

Recommended name:

- `career-voice-match-workspace`

Example structure:

- `career-voice-match-workspace/input/`
- `career-voice-match-workspace/dynamic-reference/`
- `career-voice-match-workspace/output/`

## Folder Purposes

- `input/`: store the target resume, cover letter, and any requirement notes for the current task
- `dynamic-reference/`: store user-derived voice references and optional source writing samples
- `output/`: store the revised result documents

## First-Use Interaction Flow

Follow this sequence:

1. create the workspace folders
2. ask which file should be revised
3. ask what direction the user wants the revision to go
4. tell the user that past professional writing samples are needed to match voice well
5. give a short modification plan
6. wait for user approval or added requirements
7. produce the revised file in `output/`

Do not skip the user approval step unless the user explicitly asks for immediate execution without a checkpoint.

## Working Rules

- keep static skill files unchanged during normal use
- keep dynamic user materials inside the workspace, not inside `references/`
- prefer compact derived references over large raw sample archives
- if raw samples are stored, label them as source material rather than reusable guidance
