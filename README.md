# Ripple — Build 64

Ripple combines on-device and online chat with screen selection, OCR, translation and optional capture tools.

## Download and source

- [Build 64 APK (vc167)](https://github.com/PlasticBuild/Ripple-AI/releases/tag/build64-vc167) — stable APK download release.
- [Matching complete source archive, manifest and validation](https://github.com/PlasticBuild/Ripple-AI/releases/tag/source-build64-vc167) — separate source release.
- [All releases](https://github.com/PlasticBuild/Ripple-AI/releases) · [Previous Build 63 source (vc161)](https://github.com/PlasticBuild/Ripple-AI/releases/tag/source-build63-vc161).

The APK updates the existing owner-signed Ripple installation in place. Optional chat models and the formula model are installed separately through their setup controls; downloading a tool is an explicit choice.

## Changes in Build 64

- When Google AI has no usable photo cards, fetch explicitly named photos from Google Images separately from the selected screenshot and earlier chat. Show the source; Stop cancels pending work.
- Update the existing Google reply as it grows. Add Find, jump-to-bottom and New chat controls, and keep the Google AI label readable in both themes.
- Separate capture agent/model controls, aligned header actions, OCR inspection and reviewed table export with blank-cell preservation.
- Optional local formula-to-LaTeX recognition with explicit model download/removal.
- Supported reply continuation after reported output limits; interrupted-response recovery keeps queues held for review.
- Opt-in Sassy/Rambler modes, Brave AI naming with legacy preferences retained, and retired active SearxNG choices.
- Keep manual memory tools off by default. Avoid temporary duplicate copies in photo transfers, saved chats and backups without trimming content. Explicit backend choices stay intact; manual idle release may require reloading the model for the next answer.

## Validation and limits

- 145 focused host tests across 12 classes passed. Four earlier background-preservation tests passed on code unchanged in vc167; these are separate synthetic-provider tests.
- In-place owner-signed install/normal launch passed. One phone showed lion/DDR4 Google reference cards, readable label contrast and one natural busy-queue dispatch.
- A separate Lumo 500-fact request reached the bounded 120-second timeout without visible partial text. Physical response-notification Stop/partial preservation remains unverified; no partial-loss or service defect was established.
- Earlier checks covered table review, Ghost draft/keyboard preservation, one formula setup/equation, capture controls and Local reference photos; their scope is recorded in the validation summary.
- No measured RAM/speed benefit, new NPU qualification or adaptive native-context allocation is claimed. Local backend eligibility and resource checks still apply.

See the source release’s validation and evidence summaries for the test scope and known limits. Retain the bundled component licenses and notices.
