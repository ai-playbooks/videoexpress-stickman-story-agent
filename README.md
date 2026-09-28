# VideoExpress Narrated Story Agent

Choose a fresh protagonist name for each new story rather than automatically reusing Milo. Keep the name and dedicated character master consistent throughout that story.

Design the whole action sequence before scene images: record each incoming pose, new action, outgoing pose and next scene's start. Render connected clips sequentially, using the actual accepted endpoint to finalize the following source image. Do not restart the same approach/reach from similar neutral poses. Review posture, position, gaze, contact and framing at every join; Auto Align fixes timing gaps, not repeated action. See the [continuous cat storyboard](examples/continuous-cat-story.md).

For a continuous same-location action, use Save Last Frame and load that reviewed image as the next clip's source when supported. Keep the dedicated character master as the separate consistent-character reference. This carries the actual pose and camera framing forward without regenerating a similar neutral setup.

The current route creates narration directly inside VideoExpress: **Narration Video → Create Video → CloneVoice → System Voice → voice → create audio → generate video**. Advanced Mode stays off. The motion prompt contains visual instructions only; narration belongs in the TTS dialog. Standalone CloneVoice creation, downloads, and narration-library imports are no longer the default.

Copy [SYSTEM_PROMPT.md](SYSTEM_PROMPT.md) into a browser-capable agent, sign into VideoExpress, and supply topic and ratio. Routine production continues through review, Auto Align, and saving. Mandatory tool policies and explicit account-confirmation requests remain applicable.

The current experiment uses polished 3D. Detailed images show the actual narrated moment, all necessary people/props in correct positions, and layered foreground/middle ground/background, coherent light, tactile materials, and contact shadows. Images are not mechanically forced into early setup poses. Short narration beats target natural 3–5 seconds, verified in the integrated workflow.

Every new story first generates a dedicated standalone stickman master character image. Save and review it before creating scenes, then select that same image as the Consistent Character reference for every clip, including scene 1. Scene images never replace the master. Keep the selected master through revisions of that story.

Recurring locations also have a fixed layout: exact landmark positions, neighboring objects, distances and camera side repeat in every prompt. Use a separate environment reference as Reference Photo 2 when supported, while keeping the character master in Reference Photo 1. Reject swapped or mirrored sets and compare each clip endpoint with the next image before assembly.

Choose the interaction perspective before locking the set. Participants should face and look toward each other in side-on or three-quarter views; the character master preserves identity, not a front-facing pose. Reject source images that put the interaction target behind the protagonist or make the protagonist stare into the lens. Maintain those eyelines in the animation.

See [acceptance checklist](evals/acceptance-checklist.md) and [beach example](examples/beach-visit.md). Older heist examples describe historical experiments and do not override the current prompt. Never commit credentials or private session data. Export only when requested.
