# Ripple — Build 65

- [APK download release](https://github.com/PlasticBuild/Ripple-AI/releases/tag/build65-vc179).
- [Corresponding source and validation](https://github.com/PlasticBuild/Ripple-AI/releases/tag/source-build65-vc179).

### Google AI

- Add Google AI to main chat and Assistant mode.
- Send a photo through Google AI’s chat attachment control and keep the conversation for follow-up messages.
- Keep the original Circle to Search selection visible above the Google conversation.
- Resolve photo requests such as “another one” from the Google conversation instead of searching those words literally.
- Recognize corrected photo requests and follow-up answers to photo clarification questions.
- Fix Google photo cards being rejected because image and publisher IDs differ or hidden feedback fields are present.
- Try Google Images when returned page previews cannot load, while keeping results attached to the correct reply.

### Duck.ai

- Add Duck.ai to main chat, Assistant mode and Circle to Search.
- Choose among six website model choices under one Duck.ai agent.
- Send text and a single photo when the selected model supports image uploads.
- Keep model selection separate from agent selection.
- Send messages directly from Ripple without opening a website popup.
- Duck.ai keeps the selected model through follow-up messages and reads the newest answer without confusing it with earlier replies.
- Keep completed Duck.ai capture conversations ready when switching agents, without re-uploading the original image or resending earlier messages.

### Circle to Search

- Wait for older chats to finish saving before switching agents; keep the visible chat during background preparation.
- Keep the original Circle to Search selection and unsent draft when starting a new chat.

### Automatic Copy text

- Circle or drag across an area to select equations and multiple table columns.
- Recognize likely equations automatically with the installed local formula reader, including separated exponents and symbols.
- Use repeated column alignment when nearby table headings would otherwise merge.
- Copy uncertain content as ordinary text; never substitute rejected OCR fragments as verified values.
- Leave the clipboard unchanged when formula reading fails and there is no accepted text to copy.

### Capture toolbar

- Keep the activation and live capture toolbars consistent.
- Hide optional advanced capture tools by default; enable them in Dev settings.

### Settings

- Update default settings for new installations; preserve existing saved choices.
- Add a reusable settings profile export under About → Backup and restore.
- Keep credentials, chats, account sessions and private device state out of release-default profiles.

### Release validation verified

- vc179 host checks: 235 tests across 29 suites; no failures, errors or skipped tests.
- vc179 phone update: in-place installation and normal launch passed, preserving the existing app installation.
- vc179 Circle to Search: Google-to-Duck Continue and a real follow-up retained the synthetic conversation context.
- vc179 regression fixed: after visiting Google and returning to the existing Duck.ai chat, the previously failing request completed with WRITING COMPLETE, without Retry or the visible-text error.
- vc179 testing cleanup: synthetic test chat and crop removed; original app state restored and the phone session closed.
- Retained vc178 evidence: two native capture New chat resets kept the original crop and unsent draft. These checks were not repeated on vc179; cursor position is covered by host tests.
- Retained vc178 evidence: an active main-chat Duck.ai request completed through Home and launcher return. This does not establish visible partial-token streaming or Circle to Search task re-entry.
- Retained vc177 evidence: Google New chat completed twice and one queued Duck.ai message was delivered once. These unchanged paths also have current host coverage.
- Complete source archive: integrity test, fresh extraction and file-hash verification passed; signing secrets and raw phone captures are excluded.
- This release adds no new NPU qualification or measured RAM/speed result; it does not claim every model/provider was physically retested.
- GitHub release publication and updater verification are checked separately from these local validation results.

### Files

- APK: `Ripple-Build65-vc179-r1.apk` — 319,802,876 bytes; SHA-256 `aa4242f24faa91dd382965f74e9cb035b678e9494dd42ce90e1ac6f06037b295`.
- Corresponding source: `Ripple-Build65-vc179-source.7z` — 1,006,116,931 bytes; SHA-256 `af529c59d527c0cc1122c0a5e2098583fb2655d2955332ab35c5028e251e037c`.
- [Source manifest](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build65-vc179/Ripple-Build65-vc179-source-manifest.json).
- [Validation record](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build65-vc179/Ripple-Build65-vc179-validation.json) and [evidence summary](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build65-vc179/Ripple-Build65-vc179-evidence.json).
