# Kickoff Protocol

Use this reference when the agent is starting a new resume or cover-letter tone revision task and needs a consistent first-use interaction flow.

## Goal

Make sure the agent knows how to start the task, what to ask for, when to present a plan, and when to wait for approval.

## First Message Structure

The first user-facing message should do four things:

1. confirm the target file to revise
2. confirm the requested direction of change
3. ask for past professional writing samples if no usable voice reference already exists
4. say that a short modification plan will follow before rewriting starts

Keep the message short and concrete.

## Required Questions

Before rewriting, the agent should confirm:

- which file should be revised
- what tone direction the user wants
- whether the user can provide past professional writing samples

If the target file and tone direction are already clear, only ask for the missing writing samples.

## Sample First Message

Use wording like this:

"Please share the resume or cover letter you want revised, tell me what direction you want the tone to move in, and send a few past professional writing samples so I can match your voice more accurately. Once I review them, I’ll give you a short modification plan before I start rewriting."

Adjust wording as needed, but keep the sequence intact.

## Plan Stage

After reviewing the target draft and any writing samples, give a short plan that covers:

- what file will be revised
- what tone shift will be made
- whether a reusable voice reference will be created or updated
- what kind of output will be produced

Keep the plan short. The plan is a checkpoint, not a long explanation.

## Approval Gate

After giving the plan, stop and wait for:

- `y`
- `n`
- or additional user instructions

Do not produce the final rewritten document until the user approves or explicitly asks to skip the checkpoint.

## After Approval

After approval:

1. save or organize the task materials in the workspace
2. create or update `dynamic-reference/voice-reference.md` if useful
3. revise the document
4. save the final result in `output/`
5. return the revised result to the user

## If Samples Are Missing

If the user cannot provide past writing samples:

- proceed with the target draft and explicit tone instructions
- say briefly that voice matching will be less personalized without samples
- avoid blocking the task unless the user specifically wants close voice matching
