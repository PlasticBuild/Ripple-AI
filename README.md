# Ripple — Build 67

- [Download the stable Build 67 APK (vc192)](https://github.com/PlasticBuild/Ripple-AI/releases/tag/build67-vc192).
- [Corresponding source, build recipes, licenses and validation](https://github.com/PlasticBuild/Ripple-AI/releases/tag/source-build67-vc192).
- The stable app release contains only the APK. The separate source prerelease is excluded from Latest and app updates.

### New in Build 67

- Zoom and pan captured screens with two fingers in Circle to Search, Copy text and Translate; keep text boxes and selections aligned.
- Swipe toolbars and selection bubbles between top and bottom with a smooth slide. Keep their position when switching tools on the same capture; respect reduced-motion settings.
- Read curved text lines in their original order, including numbers beneath barcodes.
- Keep Google AI photo context, display contextual reference photos and deliver queued follow-ups.
- Retain Google reply text when background page animations pause; remove empty formatting artifacts and obsolete timeout warnings when delayed replies arrive.
- Use neutral Google visual-search prompts while preserving custom prompts. Keep held messages available for explicit review.
- Choose source languages per text region on mixed-language captures.
- Cancel an attachment import with Stop while retaining the unsent draft.

### Optional Find on screen preview

- Describe an item with LOCUS-2B and review its proposed selection before using it. Some crops include surrounding content.
- Run the full model locally with Ripple's native CPU runtime; this optional feature is a preview within the stable app release.
- Download about 7.76 GB directly from pinned Hugging Face revisions. No API key is needed; these model weights are not bundled in the APK or source archive.
- Require at least 6 GiB of available memory. Release idle chat memory before loading local vision, and retire the vision worker after completion or cancellation.
- Further LOCUS crop-accuracy work and NPU integration are planned for Build 68; no LOCUS NPU acceleration or speed-up is claimed here.

### Known limitations

- Google may require its own verification or consent. Website availability and provider responses can vary.
- Local vision and OCR can omit or misread content; review proposed selections and extracted text.
- Public SearXNG support is configurable and off by default; no public JSON-enabled server has passed release qualification.
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

- Release lint, build, original signing certificate and 16 KiB alignment checks passed.
- Focused host runs passed: 72 focused animation, capture and release-catalog checks, 70 Google reply/prompt cases and 119 swipe/capture cases. These are separate scoped runs, not a combined full-suite claim.
- Phone acceptance covers 18 scoped cases: final vc192 installation, visible intermediate animation frames, zoom and cleanup, plus explicitly reviewed unchanged vc190/vc191 Google and LOCUS checks.
- Google contextual photos, queued follow-ups and background reply retention were observed. Production LOCUS setup, preview, cancellation and return to chat were observed.
- LOCUS final outputs agreed with the pinned Python reference on controlled cases; the stricter intermediate-tensor comparison remains failed. Agreement does not establish crop accuracy or performance.
- Reduced motion has focused host coverage; no separate physical reduced-motion setting test is claimed. Android instrumentation compiled; compiled-only cases are not reported as executed.
- Complete source integrity, fresh extraction and every archived file hash passed. Signing secrets, private photos and raw phone evidence are excluded.

### Files

- APK: `Ripple-Build67-vc192-r1.apk` — 292,843,416 bytes; SHA-256 `8d04f54b1d67bb54bdc274f7b50feddf0b9fd27bc74968bb557de9a2073ea24a`.
- Source: `Ripple-Build67-vc192-source.7z` — 982,056,740 bytes; SHA-256 `830e3a9a397fc171a10c427000451cda1da460fb460e650a53924c5fd2e6e2e9`.
- [Source manifest](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build67-vc192/Ripple-Build67-vc192-source-manifest.json).
- [Validation record](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build67-vc192/Ripple-Build67-vc192-validation.json) and [evidence summary](https://github.com/PlasticBuild/Ripple-AI/releases/download/source-build67-vc192/Ripple-Build67-vc192-evidence.json).

### Previous release

- [Build 66 / vc188 release](https://github.com/PlasticBuild/Ripple-AI/releases/tag/build66-vc188) and [its README and validation scope](https://github.com/PlasticBuild/Ripple-AI/blob/712a13faeaab974540130e90225acd5f2ca6c527/README.md).
