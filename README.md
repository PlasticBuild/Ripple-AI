# Ripple — Build 66

- [Download Build 66 (vc188)](https://github.com/PlasticBuild/Ripple-AI/releases/tag/build66-vc188).
- [Corresponding source, build recipes, licenses and validation](https://github.com/PlasticBuild/Ripple-AI/releases/tag/source-build66-vc188).
- The stable app release contains only the APK. The separate source prerelease is excluded from app updates.

### Known limitations

- Google AI can remain at Preparing or report verification/consent required. Photo requests and queued messages may not complete. The verification recovery fix and remaining Google photo, list-spacing and queue checks are scheduled for Build 67.
- Local vision can omit objects. The focused Hexagon test missed one object in its initial description, although its count follow-up was correct.
- LOCUS is not yet usable for live inference. Native Android LOCUS integration is the main goal for Build 67.
- Public SearXNG support is configurable and off by default; no public JSON-enabled server has passed release qualification.
- Region OCR can misread or omit characters; compare the captured text and correct it when needed.
- No all-model accuracy, general NPU speed increase, or measured RAM/latency improvement is claimed.

### AI connections and chat

- Use configured AI connections in main chat, Assistant and Circle to Search.
- Keep agent/model choices, conversation ownership, source cards and message timestamps distinct.
- Extract selected text locally for text-only connections.
- Retain unsent photo cards with draft text, restore them after reopening or Undo, and never send a restored draft automatically.
- Preserve Ghost and disabled-history choices when saving drafts.

### Circle to Search and attachments

- Recover detached activation areas and abandoned capture launches.
- Keep the original selected image separate from returned reference photos.
- Choose local page preparation for more privacy or direct background uploads for faster result switching; apply photo-sharing and Ghost preferences.
- Add custom HTTPS search websites, optional query templates and supported manual image-upload controls.
- Remove Bing, TinEye, Litterbox and Catbox routes.
- Use Photo, File or Take photo attachment actions; Photo opens Android's Photos picker.
- Optionally review Continue context and edit its latest question, summary or attachments before transferring it.

### Search, captures and translation

- Show source cards, numbered citations and retry controls for individual failed image-search sources.
- Choose Fast, Balanced or Deep research, with optional SearXNG configuration.
- Apply selected-domain and verified-date filters to Ripple's research retrieval, with explicit unsupported-path and missing-date limits.
- Group snapshots into named collections and stage questions using up to six captures.
- Choose immediate deletion or 1, 7 or 30 days of recovery for normal chats and snapshots; Ghost content stays outside recovery.
- Inspect translated regions, correct their source text or rescan a selected region.
- Omit empty detector hints from ordinary photo prompts; retain exact boxes for explicit detector review.

### Size and resource changes

- Remove native debug sections while retaining executable code, exported functions and integrity checks.
- Reduce redundant response-stream processing while preserving response limits and Stop behavior.
- Use one row of temporary pixels for sharpening and reuse unchanged chat-history records.
- View actual runtime, loading and first-response information in Settings.

### Verified scope

- 1,387 host tests across 168 suites passed without failures, errors or skipped tests.
- 11 production Google DOM fixtures passed. The separate Build 67 verification fix is not included in this APK.
- Release build, signing and 16 KiB alignment checks passed. Lint retains 736 warnings and six hints.
- Android instrumentation code compiled; device instrumentation was not executed.
- In-place vc188 installation and normal launch passed. The focused phone session observed unfolded activation and the Photos picker.
- Automatic-selected CPU and explicit Hexagon returned correct synthetic count follow-ups; their differing outputs and warm/cold states do not support a general speed comparison.
- Google crop handoff was observed, but Google reply/photo delivery and queue completion remained blocked. Repeat-photo and list-spacing checks were not run.
- Automatic compute was restored and identified synthetic test material was cleaned up.
- The complete source archive passed integrity, fresh-extraction and file-hash verification. Signing secrets and raw phone evidence are excluded.

### Files

- APK: `Ripple-Build66-vc188-r1.apk` — 286,830,076 bytes; SHA-256 `d153930ff35d2d258ba7035d6b3d1ee8ed6cfe8814c6d3e0b9d9a50e5b19814b`.
- Source: `Ripple-Build66-vc188-source.7z` — 981,786,833 bytes; SHA-256 `92ccd9bc0281b7dc0e4fa8e01cfe83d8435eaf7e586768022aa9593e84c9c4fd`.
- [Source manifest](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build66-vc188/Ripple-Build66-vc188-source-manifest.json).
- [Validation record](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build66-vc188/Ripple-Build66-vc188-validation.json) and [evidence summary](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build66-vc188/Ripple-Build66-vc188-evidence.json).
