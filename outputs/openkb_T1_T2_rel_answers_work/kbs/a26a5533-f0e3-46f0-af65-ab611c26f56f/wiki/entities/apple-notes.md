---
sources: ["summaries/session-34_2024-12-16.md"]
type: "Product"
description: "Apple's built‑in note‑taking app for iOS/macOS used as an audio hub."
---

# Apple Notes

Apple Notes is the native note‑taking application on iOS and macOS, providing a simple, sync‑enabled space for text, images, sketches, and embedded audio files. In the workflow described in [[summaries/session-34_2024-12-16]], it serves as the central "Audio Inbox" where all learning‑related artifacts—podcast clips, text‑to‑speech highlights, and voice‑note recordings—are collected for later review.

## Key Facts from Session 34
- **Audio‑first hub**: All shared items are appended to a single Notes page, allowing the user to open one document and listen to everything with minimal tapping.
- **Integration via Shortcuts**: A custom [[entities/apple-shortcuts]] shortcut named *Append to Audio Inbox* receives shared audio, text, or files from other apps and adds a timestamp before appending them to the designated note.
- **Supported sources**:
  - Podcast clips from [[entities/overcast]] (and similar apps like Airr) are shared directly to the note.
  - Highlights from articles or PDFs read with [[concepts/text-to-speech]] tools such as Voice Dream Reader are stored as plain text that can be spoken via Speak Screen.
  - Voice recordings captured in [[entities/noted]] or [[entities/audio-pen]] are saved as both raw audio and transcribed summaries.
- **Review workflow**: Open the note, enable Speak Screen (or ask Siri) to have any text read aloud, and tap embedded audio files to listen.

## Related Concepts
- [[concepts/active-listening]] – encouraging brief mental recaps while listening.
- [[concepts/shortcuts-workflow]] – automating the capture of audio and text into Notes.
- [[concepts/text-to-speech]] – extracting spoken content from written sources.
- [[concepts/triage-rule]] – deciding quickly whether to keep or discard a piece of audio based on relevance.

## Associated Entities
- [[entities/iphone]] – the primary device on which this workflow is built.
- [[entities/overcast]] – podcast app providing clip‑saving.
- [[entities/audio-pen]] – voice‑note app that transcribes recordings.
- [[entities/noted]] – alternative voice‑note capture tool.
- [[entities/voice-dream-reader]] – TTS app used for article reading.

---
*This page synthesizes information from the session‑34 summary and highlights how Apple Notes functions as a low‑effort, audio‑centric repository for personal learning.*