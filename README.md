# VideoExpress Stickman Audio-Synced Story Agent

A team-owned system prompt for creating colorful stickman stories from short audio/video pairs: one narration line, one separate 3–5 second CloneVoice audio clip, and one matching silent VideoExpress scene. Characters stay consistent, and each video starts and ends with its paired audio. The default look is 2D; a requested 3D version uses a new 3D master and 3D scene images while keeping the audio-first timing workflow.

For a one-minute story, plan approximately 15 pairs averaging 4 seconds each (12–20 pairs depending on actual audio durations). Measure each generated audio clip before making its video. If generation duration controls cannot match it exactly, generate a covering video and trim only the excess video tail. Assemble the pairs consecutively and verify every boundary.

## Use

1. Open [SYSTEM_PROMPT.md](SYSTEM_PROMPT.md).
2. Copy the complete prompt into Codex or another browser-capable agent.
3. Enable its supported browser or computer-control capability and keep production browsing visible.
4. Sign in to CloneVoice and VideoExpress yourself when requested.
5. Send the two required inputs shown in [examples/example-request.md](examples/example-request.md): a topic/story and an aspect ratio.

A target runtime may also be supplied. Actual audio measurements determine scene timing; word-count estimates do not determine timeline boundaries.

The agent first opens or focuses a visible browser, using your selected session or preferring the built-in browser. If that fails, it tries other available supported browsers and signed-in sessions before requesting troubleshooting. Requested account confirmation happens before generation and is retained for that session.

Topic and aspect ratio authorize routine production through a saved, verified project, including separate CloneVoice audio creation. The agent does not ask permission for every clip or phase. A prechecked terms box alone is not treated as evidence of a new agreement; mandatory action-time confirmations still apply when an action actually accepts an agreement. Recoverable failures get 2–3 informed attempts before a detailed request for help.

Workflow preferences live in `SYSTEM_PROMPT.md` so they travel with the prompt across conversations and devices. They remain subject to the active agent's tool and policy requirements.

## Contents

For cinematic action and comedy, prompts specify one decisive action, one motivated camera move, and a visible consequence per audio beat. The experimental [clumsy diamond heist](examples/clumsy-diamond-heist.md) targets 30–40 seconds in 16:9 while retaining the same audio-first synchronization workflow. A 3D remake can reuse accepted narration while generating a separate 3D master and eight new shots. The active VideoExpress model is used without changing providers.

- `SYSTEM_PROMPT.md` — the complete production-agent prompt
- `examples/example-request.md` — a paste-ready sample request
- `evals/acceptance-checklist.md` — the production acceptance checklist

## Security

Never place CloneVoice or VideoExpress passwords, GitHub credentials, tokens, API keys, or browser-session data in this repository. Users sign in through the normal browser login flow.
